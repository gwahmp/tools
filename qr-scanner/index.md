---
layout: default
---
<link rel="stylesheet" href="css/style.css"/>
<div class="container py-0 py-sm-5 mt-1">
    <div class="row justify-content-center">
        <div id="qr-result"></div>
        <div class="col-md-6 text-center scanner">
            <div class="scan"></div>
            <video id="video" class="border rounded" style="width: 100%; height: auto;"></video>
            <button id="scan-btn" class="btn btn-primary btn-lg col-12 mt-3 px-5">Scan QR</button>
            <canvas id="canvas" class="d-none"></canvas>
        </div>
    </div>
</div>


<script src="js/qrscan.js"></script>
<script src="js/qrscript.js"></script>
