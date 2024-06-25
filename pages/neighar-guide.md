---
layout: page
title: Neighar Guide
permalink: /neighar-guide/
comments: false
---

### What is Neighar?

<button onclick="showGif('v1')">Toggle 1</button>
<button onclick="showGif('v2')">Toggle 2</button>
<button onclick="showGif('v3')">Toggle 3</button>

<div id="v1" style="text-align:center;">
    <img src="{{ '/assets/videos/1.gif' | relative_url }}" alt="My SVG Video" width="400">
</div>
<div id="v2" style="text-align:center; display:none;">
    <img src="{{ '/assets/videos/1.gif' | relative_url }}" alt="My SVG Video" width="400">
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
}
</script>
