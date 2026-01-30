---
title: About
layout: index
section: about
language: ko-KR
base_url: index.html

h2_title: 29th Roboracer Autonomous Racing Competition

---

ROBORACER Grand Prix는 연구원, 엔지니어 및 자율 시스템 엔지니어로 구성된 국제 커뮤니티가 주최하는 대회입니다.

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

IFAC 2026에서 열리는 29th Roboracer Autonomous Racing Competition에 참가하는 팀은 주어진 사양에 따라 1:10 규모의 자율 주행 자동차를 제작하고 대회 목표를 달성하기 위한 소프트웨어를 작성합니다.
<br>
<br>
IFAC 2026는 대면 경쟁으로 대회를 진행합니다.
<br>
<br>
대면 경쟁: 이 형태는 한국의 부산에서 대면으로 대회에 참가하는 참가자를 대상으로 합니다. 각 팀은 자신의 소프트웨어와 함께 실제 ROBORACER 차량을 가져옵니다. 주최 측은 경주 설정(규칙, 제출, 지침), 트랙, 관련 인프라를 제공하고 레이스 자체를 구성합니다.
<br>
<br>

<!-- <center>
<a href="https://2023.iccas.org/" class="image main"><img src="../images/iccas.png"  style="width: 25vw" alt="국제제어자동화로봇시스템학회" /></a>
</center>
<br>
<center>
<a href="#" class="image main"><img src="../images/F1TENTH/f1tenth_korea_logo.jpg"  style="width: 35vw" alt="" /></a>
</center> -->
<br>
<br>
<center>
  <h3>이전 대회 영상</h3>
  <iframe style="width: 35vw; aspect-ratio: 16/9;" src="https://www.youtube.com/embed/tnn4isfdUCE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</center>
<br>