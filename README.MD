<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Bhawan’s Animation Portfolio</title>
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body {
      font-family: 'Segoe UI', sans-serif;
      background: #121212;
      color: #f1f1f1;
      scroll-behavior: smooth;
    }
    header {
      height: 100vh;
      background: linear-gradient(to bottom right, #1f1f1f, #0a0a0a);
      display: flex;
      align-items: center;
      justify-content: center;
      flex-direction: column;
      text-align: center;
      padding: 20px;
    }
    header h1 {
      font-size: 3rem;
      color: #ffcc70;
      animation: fadeIn 2s ease-out;
    }
    header img {
      width: 150px;
      border-radius: 50%;
      margin: 20px 0;
      box-shadow: 0 0 20px #ffcc70;
    }
    section {
      padding: 60px 20px;
      max-width: 1000px;
      margin: auto;
      animation: fadeInUp 1s ease-out;
    }
    h2 {
      margin-bottom: 20px;
      color: #ffcc70;
    }
    .projects {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 20px;
    }
    .card {
      background: #1f1f1f;
      padding: 10px;
      border-radius: 12px;
      overflow: hidden;
      transition: transform 0.3s ease;
      cursor: pointer;
    }
    .card:hover {
      transform: scale(1.05);
    }
    .card img, .card video {
      width: 100%;
      border-radius: 10px;
    }

    .modal {
      display: none;
      position: fixed;
      z-index: 999;
      top: 0; left: 0;
      width: 100%; height: 100%;
      background: rgba(0, 0, 0, 0.8);
      justify-content: center;
      align-items: center;
    }
    .modal-content {
      max-width: 90%;
      max-height: 90%;
    }
    .modal.show {
      display: flex;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(-20px); }
      to { opacity: 1; transform: translateY(0); }
    }
    @keyframes fadeInUp {
      from { opacity: 0; transform: translateY(50px); }
      to { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>
<body>

  <header>
    <h1>Animation by Bhawan</h1>
    <img src="momo-face.gif" alt="Bhawan Profile" />
    <p>Where Art Comes to Life</p>
  </header>

  <section id="projects">
    <h2>Projects</h2>
    <div class="projects">
      <div class="card" onclick="openModal('rigged_cloths_3.mp4', true)">
        <video src="rigged_cloths_3.mp4" muted autoplay loop></video>
      </div>
      <div class="card" onclick="openModal('elements-2.gif', false)">
        <img src="elements-2.gif" alt="Illustration" />
      </div>
    </div>
  </section>

  <div class="modal" id="modal">
    <div class="modal-content" id="modalContent"></div>
  </div>

  <script>
    const modal = document.getElementById('modal');
    const modalContent = document.getElementById('modalContent');

    function openModal(src, isVideo) {
      modal.innerHTML = isVideo ?
        <video controls autoplay src="${src}" style="max-width:100%; border-radius:10px;"></video> :
        <img src="${src}" style="max-width:100%; border-radius:10px;">;
      modal.classList.add('show');
    }

    modal.addEventListener('click', () => {
      modal.classList.remove('show');
      modal.innerHTML = '';
    });
  </script>
</body>
</html>
