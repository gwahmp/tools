---
layout: default
title: QR Code ScannerOnline | Scan QR Codes Instantly & Securely
description: Free web-based QR scanner tool. Instantly scan QR codes securely with no app download. Explore benefits, use cases, and step-by-step usage guide.
date: 2024-12-18
noindex: false
---
<link rel="stylesheet" href="/tools/social-post-generator/css/style.css">
<div class="container">
  <div class="row">
    {% for post in site.posts %}
      <div class="col-md-4 mb-4">
        <div class="card post-item" data-type="{{ post.media_type }}" data-src="{{ post.media_src }}" data-text="{{ post.overlay_text }}">
          <div class="media-preview position-relative">
            {% if post.media_type == "image" %}
              <img src="/tools/social-post-generator/images/{{ post.media_src }}" class="img-fluid">
            {% elsif post.media_type == "video" %}
              <video src="/tools/social-post-generator/videos/{{ post.media_src }}" class="img-fluid" muted autoplay loop></video>
            {% endif %}
            <div class="overlay-text position-absolute text-white p-2 w-100 text-center"></div>
            <div class="brand-overlay position-absolute bottom-0 start-0 text-white p-2">
              <img class="brand-logo" src="" style="max-height: 40px;">
              <span class="brand-name ms-2 fw-bold"></span>
            </div>
          </div>
          <div class="card-body">
            <button class="btn btn-sm btn-primary download-btn">Download</button>
            <div class="btn-group">
              <button class="btn btn-sm btn-secondary dropdown-toggle" data-bs-toggle="dropdown">Share</button>
              <ul class="dropdown-menu">
                <li><a class="dropdown-item share-facebook" href="#">Facebook</a></li>
                <li><a class="dropdown-item share-linkedin" href="#">LinkedIn</a></li>
                <li><a class="dropdown-item share-twitter" href="#">Twitter</a></li>
                <li><a class="dropdown-item share-whatsapp" href="#">WhatsApp</a></li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    {% endfor %}
  </div>
</div>


<script src="https://cdn.jsdelivr.net/npm/@ffmpeg/ffmpeg@0.11.6/dist/ffmpeg.min.js"></script>

<script src="https://cdn.jsdelivr.net/npm/html2canvas@1.4.1/dist/html2canvas.min.js"></script>

<script src="/tools/social-post-generator/js/main.js">
