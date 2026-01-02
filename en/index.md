---
title: About
layout: index
section: about
language: en-US
base_url: index.html
h2_title: 29th Roboracer Autonomous Racing Competition

---

ROBORACER Grand Prix is a competition organized by an international community of researchers, engineers, and autonomous systems enthusiasts.

<br>
<br>

<!-- <center>
<a href="#" class="image main"><img src="../images/roboracer.gif"  style="width: 35vw" alt="" /></a>
</center> -->

<center>
  <div style="position: relative; width: 35vw;">
    <video id="loopVideo" autoplay loop muted playsinline style="width: 100%;">
      <source src="../images/roboracer.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
    <div id="fadeOverlay"
         style="position: absolute; top: 0; left: 0; width: 100%; height: 96%;
                background: black; opacity: 0; transition: opacity 0.5s;"></div>
  </div>
</center>

<script>
  const video = document.getElementById("loopVideo");
  const overlay = document.getElementById("fadeOverlay");

  video.addEventListener("timeupdate", () => {
    if (video.duration - video.currentTime < 0.5) {
      overlay.style.opacity = 1;
    }
    else if (video.currentTime < 0.5) {
      overlay.style.opacity = 0;
    }
  });
</script>

The teams participating in 29th Roboracer Autonomous Racing Competition at IFAC 2026 will build a 1:10 scaled autonomous race car according to a given specification and write software for it to fulfill the objectives for the competition.
<br>
<br>
IFAC 2026 will be held as an in-person competition.
<br>
<br>
In-person competition: This variant targets participants who will travel to Busan, Republic of Korea. Each team will bring their own physical ROBORACER car with their software. The organizers provide the race setup (rules, submissions, guidelines), the track, related infrastructure and organize the race itself.
<br>


<!-- <br>
<center>
<a href="https://2023.iccas.org/" class="image main"><img src="../images/iccas.png"  style="width: 25vw" alt="국제제어자동화로봇시스템학회" /></a>
</center>
<br>
<center>
<a href="#" class="image main"><img src="../images/F1TENTH/ROBORACER_korea_logo.jpg"  style="width: 35vw" alt="" /></a>
</center> -->

