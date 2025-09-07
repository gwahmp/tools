---
layout: default
title: LocalChat
description: Private local chat
date: 2024-12-18
noindex: false
---

<link rel="stylesheet" href="/tools/localchat/assets/css/style.css"/>
<div id="app" class="container-fluid h-100">
    <div class="row h-100">
      <!-- Sidebar -->
      <div id="sideBarCollapse" class="col-md-4 col-lg-3 border-end p-0 sidebar d-md-block">
        <div class="p-3 border-bottom bg-light">
          <div class="d-flex gap-2 align-items-center mb-3">
            <div class="d-flex flex-grow-1 align-items-center">
              <a href="https://www.wikimint.com"><img width="50" height="30" src="/assets/images/wikimint-icon.webp"/></a> <h1 class="fs-4 ms-2 lead fw-normal text-black">LocalChat</h1>
            </div>
            <button class="btn d-none" type="button" data-bs-toggle="collapse" data-bs-target="#sideBarCollapse">
            <i class="bi bi-x-lg text-dark fs-3"></i>
          </button>
           <button id="open-settings" class="btn btn-outline-secondary" title="Settings"><i class="bi bi-gear"></i></button>
          </div>
          <div class="d-flex gap-2">
            <div class="flex-grow-1">
              <input id="search-input" class="form-control d-none" placeholder="Search contacts & groups">
            </div>
            <div>
              <!-- <button id="open-settings" class="btn btn-outline-secondary" title="Settings"><i class="bi bi-gear"></i></button> -->
            </div>
          </div>
          <div class="mt-3">
            <div class="mb-2 small text-muted">Your chat link (share)</div>
            <div class="input-group mb-2">
              <input type="text" id="my-link" class="form-control" readonly>
              <button class="btn btn-outline-secondary" id="copy-my-link"><i class="bi bi-clipboard"></i></button>
            </div>
            <div class="mb-2 small text-muted d-none">Create / Open group</div>
            <div class="input-group d-none">
              <input type="text" id="room-input" class="form-control" placeholder="group name">
              <button class="btn btn-outline-secondary" id="open-room"><i class="bi bi-people"></i></button>
              <button class="btn btn-outline-primary" id="new-group-btn" title="New Group"><i class="bi bi-plus-lg"></i></button>
            </div>
          </div>
        </div>
        <div class="p-3 flex-grow-1 overflow-auto">
          <div id="sidebar-list" class="list-group"></div>
        </div>
        <div class="p-3 small text-muted border-top">
          <strong>Note</strong>: You can chat with people on the same Wi-Fi or LAN. All chats are stored on your local devices only.
        </div>
      </div>
      <!-- Chat panel -->
      <div class="col-md-8 col-lg-9 p-0">
        <div class="d-flex align-items-center px-3 py-2 border-bottom bg-light">
          <div class="avatar-circle me-2"></div>
          <div class="flex-grow-1">
            <h6 id="chat-title" class="mb-0">LocalChat</h6>
            <small id="chat-sub" class="text-muted d-none">Select a contact or group</small>
            <div id="typing-line" class="typing-indicator d-none"></div>
            <small id="status"></small>
          </div>
          <div class="text-end d-none">
            <small id="peer-status" class="text-muted"></small>
          </div>
          <button class="btn d-md-none" type="button" data-bs-toggle="collapse" data-bs-target="#sideBarCollapse">
            <i class="bi bi-x-lg text-dark fs-3"></i>
          </button>
        </div>
        <div id="chat-messages" class="flex-grow-1 overflow-auto p-3 bg-white"></div>
        <div class="px-3 py-2 border-top bg-light">
          <div class="input-group">
            <input type="text" id="message-input" class="form-control" placeholder="Type a message...">
            <button id="send-btn" class="btn btn-primary"><i class="bi bi-send"></i></button>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- Save Contact Modal -->
  <div class="modal fade" id="saveContactModal" tabindex="-1" aria-hidden="true">
    <div class="modal-dialog">
      <form id="save-contact-form" class="modal-content">
        <div class="modal-header">
          <h5 class="modal-title">Save Contact</h5>
          <button type="button" class="btn-close" data-bs-dismiss="modal"></button>
        </div>
        <div class="modal-body">
          <p>Add device: <code id="link-uuid-display"></code></p>
          <div class="mb-3">
            <label class="form-label">Name</label>
            <input type="text" id="contact-name" class="form-control" required>
          </div>
        </div>
        <div class="modal-footer">
          <button class="btn btn-secondary" type="button" data-bs-dismiss="modal">Cancel</button>
          <button class="btn btn-primary" type="submit">Save</button>
        </div>
      </form>
    </div>
  </div>

  <!-- New Group Modal -->
  <div class="modal fade" id="newGroupModal" tabindex="-1" aria-hidden="true">
    <div class="modal-dialog">
      <form id="new-group-form" class="modal-content">
        <div class="modal-header">
          <h5 class="modal-title">Create New Group</h5>
          <button type="button" class="btn-close" data-bs-dismiss="modal"></button>
        </div>
        <div class="modal-body">
          <div class="mb-3">
            <label class="form-label">Group Name</label>
            <input type="text" id="group-name" class="form-control" required>
          </div>
          <div class="mb-2">Select Members</div>
          <div id="modal-contact-list" class="list-group" style="max-height:320px; overflow:auto;"></div>
        </div>
        <div class="modal-footer">
          <button class="btn btn-secondary" data-bs-dismiss="modal" type="button">Cancel</button>
          <button class="btn btn-primary" id="create-group-btn" type="submit">Create Group</button>
        </div>
      </form>
    </div>
  </div>

  <!-- Settings Modal -->
  <div class="modal fade" id="settingsModal" tabindex="-1" aria-hidden="true">
    <div class="modal-dialog">
      <form id="settings-form" class="modal-content">
        <div class="modal-header">
          <h5 class="modal-title">Profile Settings</h5>
          <button type="button" class="btn-close" data-bs-dismiss="modal"></button>
        </div>
        <div class="modal-body">
          <div class="mb-3">
            <label class="form-label">Display Name</label>
            <input type="text" id="my-name" class="form-control">
          </div>
          <div class="mb-3 d-none">
            <label class="form-label">Your User ID (readonly)</label>
            <input type="text" id="my-uuid" class="form-control" readonly>
          </div>
        </div>
        <div class="modal-footer">
          <button class="btn btn-secondary" data-bs-dismiss="modal" type="button">Close</button>
          <button class="btn btn-primary" type="submit">Save</button>
        </div>
      </form>
    </div>
  </div>

<div class="d-none">
<!-- hidden audio element -->
<audio id="msgSent" preload="auto" style="display:none;">
  <source src="/tools/localchat/assets/audio/ms.mp3" type="audio/mpeg">
</audio>

<!-- hidden audio element -->
<audio id="msgReceived" preload="auto" style="display:none;">
  <source src="/tools/localchat/assets/audio/mr.mp3" type="audio/mpeg">
</audio>

</div>
<!-- dependencies -->
<script src="https://unpkg.com/dexie@3.2.4/dist/dexie.min.js"></script>
<script src="https://unpkg.com/peerjs@1.5.2/dist/peerjs.min.js"></script>

<script src="/tools/localchat/assets/js/server.js"></script>
