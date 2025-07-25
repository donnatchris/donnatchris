<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>42 Portfolio – Christophe Donnat</title>
  <style>
    body {
      font-family: sans-serif;
      background: #0b0c10;
      color: #e5e5e5;
      padding: 2rem;
    }

    h1 {
      text-align: center;
      margin-bottom: 2rem;
    }

    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(160px, 1fr));
      gap: 1.5rem;
      max-width: 1000px;
      margin: auto;
    }

    .project {
      text-align: center;
    }

    .project-title {
      margin-bottom: 0.5rem;
    }

    .project-title a {
      color: #61dafb;
      text-decoration: none;
      font-weight: bold;
    }

    .project-title a:hover {
      text-decoration: underline;
    }

    .project img {
      width: 100%;
      max-width: 160px;
      border-radius: 10px;
      cursor: zoom-in;
      transition: transform 0.2s ease;
    }

    .project img:hover {
      transform: scale(1.05);
    }

    /* Lightbox */
    .lightbox {
      display: none;
      position: fixed;
      z-index: 999;
      top: 0; left: 0;
      width: 100%;
      height: 100%;
      background: rgba(0,0,0,0.9);
      justify-content: center;
      align-items: center;
    }

    .lightbox img {
      max-width: 90%;
      max-height: 90%;
      border-radius: 12px;
    }

    .lightbox:target {
      display: flex;
    }

    .lightbox-close {
      position: absolute;
      top: 30px;
      right: 40px;
      color: white;
      font-size: 2rem;
      text-decoration: none;
      font-weight: bold;
    }

    .note {
      margin-top: 2rem;
      text-align: center;
      font-style: italic;
      color: #bbb;
    }
  </style>
</head>
<body>

  <h1>🐙 42 Portfolio – Christophe Donnat</h1>

  <div class="gallery">
    <!-- Exemple d’un projet -->
    <div class="project">
      <div class="project-title">
        <a href="https://github.com/chdonnat/transcendance-42" target="_blank">Transcendance</a>
      </div>
      <a href="#lightbox-transcendance">
        <img src="images/transcendance_vignette.png" alt="Transcendance">
      </a>
    </div>

    <!-- Répète pour chaque projet -->
    <div class="project">
      <div class="project-title">
        <a href="https://github.com/chdonnat/inception-42" target="_blank">Inception</a>
      </div>
      <a href="#lightbox-inception">
        <img src="images/inception_vignette.png" alt="Inception">
      </a>
    </div>

    <div class="project">
      <div class="project-title">
        <a href="https://github.com/chdonnat/webserv-42" target="_blank">Webserv</a>
      </div>
      <a href="#lightbox-webserv">
        <img src="images/webserv_vignette.png" alt="Webserv">
      </a>
    </div>

    <div class="project">
      <div class="project-title">
        <a href="https://github.com/chdonnat/piscine-cpp-42" target="_blank">Piscine C++</a>
      </div>
      <a href="#lightbox-cpp">
        <img src="images/piscine-cpp_vignette.png" alt="Piscine C++">
      </a>
    </div>

    <!-- Ajoute ici les autres projets exactement dans le même style -->

  </div>

  <!-- Lightboxes -->
  <div id="lightbox-transcendance" class="lightbox">
    <a href="#" class="lightbox-close">&times;</a>
    <img src="images/transcendance_vignette.png" alt="Transcendance">
  </div>

  <div id="lightbox-inception" class="lightbox">
    <a href="#" class="lightbox-close">&times;</a>
    <img src="images/inception_vignette.png" alt="Inception">
  </div>

  <div id="lightbox-webserv" class="lightbox">
    <a href="#" class="lightbox-close">&times;</a>
    <img src="images/webserv_vignette.png" alt="Webserv">
  </div>

  <div id="lightbox-cpp" class="lightbox">
    <a href="#" class="lightbox-close">&times;</a>
    <img src="images/piscine-cpp_vignette.png" alt="Piscine C++">
  </div>

  <p class="note">
    🖼️ All thumbnails are original illustrations made for each project.<br>
    Some are cute. Some are cursed. All are tentacular.
  </p>

</body>
</html>


