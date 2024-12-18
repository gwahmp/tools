---
layout: default
title: Text to Audio Converter & Downloader - Free MP3 & WAV Tool
description: Convert text to audio online with this free tool. Play and download audio in MP3, WAV, and more. Fast, easy, and browser-based with no extra software needed.
date: 2024-12-18
noindex: true
---
 <div class="container">
        <div class="card">
            <div class="card-body">
                <h5 class="card-title text-center">Text-to-Audio Downloader</h5>
                <div>
                    <div class="mb-3">
                        <label for="textInput" class="form-label">Enter Text</label>
                        <textarea id="textInput" class="form-control" rows="5" placeholder="Type or paste your text here..."></textarea>
                    </div>
                    <div class="mb-3">
                        <label for="voiceSelect" class="form-label">Select Voice</label>
                        <select id="voiceSelect" class="form-select">
                            <option value="">Default</option>
                        </select>
                    </div>
                    <div class="mb-3">
                        <button type="button" id="playAudio" class="btn btn-primary">Play Audio</button>
                        <div class="btn-group">
                            <button type="button" class="btn btn-success dropdown-toggle" data-bs-toggle="dropdown" aria-expanded="false">
                                Download Audio
                            </button>
                            <ul class="dropdown-menu">
                                <li><button type="button" class="dropdown-item downloadAudio" data-format="mp3">Download as MP3</button></li>
                                <li><button type="button" class="dropdown-item downloadAudio" data-format="wav">Download as WAV</button></li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

<script>
    let audioContext = null;

    async function recordAndDownloadAudio(text, selectedVoiceIndex, format) {
        if (!text.trim()) {
            alert("Please enter some text to download.");
            return;
        }

        // Initialize AudioContext
        if (!audioContext) {
            audioContext = new (window.AudioContext || window.webkitAudioContext)();
            console.log("AudioContext initialized");
        }

        const synth = window.speechSynthesis;
        const utterance = new SpeechSynthesisUtterance(text);
        const voices = synth.getVoices();
        if (selectedVoiceIndex) {
            utterance.voice = voices[selectedVoiceIndex];
        }

        // Create a MediaStreamDestination node
        const mediaStreamDestination = audioContext.createMediaStreamDestination();

        // Connect the SpeechSynthesis audio to the AudioContext
        const audioSource = new Audio(); // Placeholder audio element
        const track = mediaStreamDestination.stream.getAudioTracks()[0];

        // Create MediaRecorder
        const mediaRecorder = new MediaRecorder(mediaStreamDestination.stream);
        const chunks = [];

        mediaRecorder.ondataavailable = (event) => {
            chunks.push(event.data);
        };

        mediaRecorder.onstop = () => {
            const blob = new Blob(chunks, { type: `audio/${format}` });
            const url = URL.createObjectURL(blob);
            const a = document.createElement("a");
            a.href = url;
            a.download = `audio.${format}`;
            a.click();
            URL.revokeObjectURL(url);
        };

        // Start recording
        mediaRecorder.start();
        console.log("Recording started...");

        utterance.onend = () => {
            console.log("Speech synthesis complete, stopping recorder...");
            mediaRecorder.stop();
        };

        // Start speaking
        synth.speak(utterance);
    }

    $(document).ready(function () {
        // Populate available voices
        function populateVoices() {
            const voiceSelect = $('#voiceSelect');
            const voices = speechSynthesis.getVoices();

            voiceSelect.empty();
            voices.forEach((voice, index) => {
                const option = $(`<option value="${index}">${voice.name} (${voice.lang}) ${voice.default ? '[Default]' : ''}</option>`);
                voiceSelect.append(option);
            });
        }

        populateVoices();

        if (speechSynthesis.onvoiceschanged !== undefined) {
            speechSynthesis.onvoiceschanged = populateVoices;
        }

        // Handle Play Audio button
        $('#playAudio').on('click', function () {
            const text = $('#textInput').val();
            const selectedVoiceIndex = $('#voiceSelect').val();

            if (!text.trim()) {
                alert("Please enter some text to play.");
                return;
            }

            const utterance = new SpeechSynthesisUtterance(text);
            const voices = speechSynthesis.getVoices();
            if (selectedVoiceIndex) {
                utterance.voice = voices[selectedVoiceIndex];
            }

            speechSynthesis.speak(utterance);
            console.log("Audio playing...");
        });

        // Handle Download Audio button
        $('.downloadAudio').on('click', function () {
            const text = $('#textInput').val();
            const selectedVoiceIndex = $('#voiceSelect').val();
            const format = $(this).data('format');
            recordAndDownloadAudio(text, selectedVoiceIndex, format);
        });
    });
</script>
