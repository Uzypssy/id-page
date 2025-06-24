<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Taupo-nui-a-tia College ID Page</title>
<style>
  body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background-color: #000000;
    color: #ffffff;
    margin: 0;
  }
  header {
    background-color: #111111;
    color: #00ccff;
    padding: 20px 40px;
    text-align: center;
  }
  header h1 {
    margin: 0;
    font-weight: 700;
    font-size: 2em;
  }
  main {
    max-width: 900px;
    margin: 40px auto;
    background: #1a1a1a;
    padding: 30px 40px;
    border-radius: 8px;
    box-shadow: 0 4px 12px rgba(0, 204, 255, 0.3);
    text-align: center;
  }
  main h2 {
    margin-top: 0;
    color: #00ccff;
  }
  .profile-image {
    max-width: 300px;
    display: block;
    margin: 20px auto;
    border-radius: 8px;
    box-shadow: 0 0 15px rgba(0, 204, 255, 0.5);
    cursor: pointer;
    transition: transform 0.3s ease;
  }
  .profile-image:hover {
    transform: scale(1.05);
  }
  #popup {
    display: none;
    position: fixed;
    top: 0; left: 0;
    width: 100%; height: 100%;
    background: rgba(0,0,0,0.9);
    justify-content: center;
    align-items: center;
    z-index: 1000;
  }
  #popupContent {
    position: relative;
    max-width: 90%;
    max-height: 90%;
  }
  #popupContent img {
    width: 100%;
    height: auto;
    border-radius: 10px;
    box-shadow: 0 0 30px #00ccff;
  }
  #closeBtn {
    position: absolute;
    top: -10px;
    right: -10px;
    font-size: 32px;
    background: #00ccff;
    color: black;
    border: none;
    border-radius: 50%;
    width: 40px;
    height: 40px;
    cursor: pointer;
    line-height: 1;
  }
  #closeBtn:hover {
    background: #00ffff;
  }
  footer {
    background-color: #111111;
    text-align: center;
    padding: 20px;
    font-size: 0.9em;
    color: #777;
    margin-top: 60px;
  }
</style>
</head>
<body>

<header>
  <h1>Taupo-nui-a-tia College</h1>
</header>

<main>
  <h2>My ID</h2>
  <img src="https://i.imgur.com/0y8Ftya.jpg" alt="My ID" class="profile-image" onclick="openPopup()" />
  <p>Click the ID photo to view larger.</p>
</main>

<div id="popup" onclick="closePopup()">
  <div id="popupContent" onclick="event.stopPropagation()">
    <button id="closeBtn" onclick="closePopup()">×</button>
    <img src="https://i.imgur.com/0y8Ftya.jpg" alt="My ID Large" />
  </div>
</div>

<footer>
  &copy; 2025 Taupo-nui-a-tia College
</footer>

<script>
  function openPopup() {
    document.getElementById('popup').style.display = 'flex';
  }
  function closePopup() {
    document.getElementById('popup').style.display = 'none';
  }
</script>

</body>
</html>
# id-page
