---
layout: page
title: Neighar Guide
permalink: /neighar-guide/
comments: false
---

### What is Neighar?

<button onclick="navigateGif('prev')">&lt; Back</button>
<span id="gifName">GIF 1</span>
<button onclick="navigateGif('next')">Next &gt;</button>

<div id="v1" style="text-align:center;">
    <img src="{{ '/assets/videos/1.gif' | relative_url }}" alt="My SVG Video" width="400">
</div>
<div id="v2" style="text-align:center; display:none;">
    <img src="{{ '/assets/videos/2.gif' | relative_url }}" alt="My SVG Video" width="400">
</div>
<div id="v3" style="text-align:center; display:none;">
    <img src="{{ '/assets/videos/1.gif' | relative_url }}" alt="My SVG Video" width="400">
</div>

### Foster a safer neighborhood with Neighar

Neighar prioritizes your well-being by ensuring that all members are verified neighbors. Stay informed about the latest local events, weather forecasts, or security concerns, and actively contribute to the safety of your community.

<script>
function showGif(gifId) {
  // Hide all GIFs
  var gifElements = document.querySelectorAll('div[id^="v"]');
  gifElements.forEach(function(gif) {
    gif.style.display = 'none';
  });

  // Show the selected GIF
  var selectedGif = document.getElementById(gifId);
  if (selectedGif) {
    selectedGif.style.display = 'block';
  }
    // Update GIF name
  document.getElementById('gifName').textContent = gifNames[currentGifIndex];
}
function navigateGif(direction) {
  if (direction === 'next') {
    currentGifIndex = (currentGifIndex % totalGifs) + 1;
  } else if (direction === 'prev') {
    currentGifIndex = (currentGifIndex - 2 + totalGifs) % totalGifs + 1;
  }

  showGif('v' + currentGifIndex);
}

// Initial display setup
document.addEventListener('DOMContentLoaded', function() {
  showGif('v1');
});
</script>
