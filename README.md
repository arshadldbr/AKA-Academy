<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>AKA Academy Tool</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: #f3f4f6;
      color: #111827;
    }
    .splash {
      background: #4f46e5;
      color: white;
      text-align: center;
      padding: 80px 20px;
      border-bottom-left-radius: 40px;
      border-bottom-right-radius: 40px;
    }
    .splash h1 {
      font-size: 2.5em;
      margin-bottom: 10px;
    }
    .nav {
      display: flex;
      justify-content: space-around;
      background: #ffffff;
      box-shadow: 0 -2px 10px rgba(0, 0, 0, 0.1);
      position: fixed;
      bottom: 0;
      width: 100%;
      padding: 10px 0;
      border-top-left-radius: 20px;
      border-top-right-radius: 20px;
    }
    .nav button {
      background: none;
      border: none;
      font-size: 1em;
      color: #4f46e5;
      cursor: pointer;
    }
    .section {
      padding: 20px;
    }
    .card {
      background: white;
      margin: 15px 0;
      padding: 15px;
      border-radius: 16px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
    }
    .hidden {
      display: none;
    }
  </style>
</head>
<body>
  <div class="splash">
    <h1>Welcome to AKA Academy!</h1>
    <p>Stylish Tool for Sharing Tech Content</p>
  </div>  <div class="section" id="articles">
    <div class="card">Sample Article: How AI is Changing the World</div>
  </div>  <div class="section hidden" id="drive">
    <div class="card">Google Drive Link: <a href="#">Click here</a></div>
  </div>  <div class="section hidden" id="apps">
    <div class="card">Unlocked App: Pro Editor APK</div>
  </div>  <div class="section hidden" id="bundles">
    <div class="card">Editing Bundle: Reel Effects Pack</div>
  </div>  <div class="nav">
    <button onclick="showSection('articles')">Articles</button>
    <button onclick="showSection('drive')">Drive Links</button>
    <button onclick="showSection('apps')">Apps</button>
    <button onclick="showSection('bundles')">Bundles</button>
  </div>  <script>
    function showSection(id) {
      const sections = document.querySelectorAll('.section');
      sections.forEach(section => section.classList.add('hidden'));
      document.getElementById(id).classList.remove('hidden');
    }
  </script></body>
</html>
