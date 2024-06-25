---
layout: page
title: Neighar Guide
permalink: /neighar-guide/
comments: false
---

### What is Neighar?

<button onclick="toggleGif('v1')">Toggle 1</button>
<button onclick="toggleGif('v2')">Toggle 2</button>
<button onclick="toggleGif('v3')">Toggle 3</button>

<div id="v1" style="text-align:center;">
    <img src="{{ '/assets/videos/1.gif' | relative_url }}" alt="My SVG Video" width="400">
</div>
<div id="v2" style="text-align:center;">
    <img src="{{ '/assets/videos/1.gif' | relative_url }}" alt="My SVG Video" width="400">
</div>
<div id="v3" style="text-align:center;">
    <img src="{{ '/assets/videos/1.gif' | relative_url }}" alt="My SVG Video" width="400">
</div>

### Foster a safer neighborhood with Neighar

Neighar prioritizes your well-being by ensuring that all members are verified neighbors. Stay informed about the latest local events, weather forecasts, or security concerns, and actively contribute to the safety of your community.

<script>
function toggleGif(gifId) {
  var gifElement = document.getElementById(gifId);
  if (gifElement.style.display === 'none') {
    gifElement.style.display = 'block';
  } else {
    gifElement.style.display = 'none';
  }
}
</script>
