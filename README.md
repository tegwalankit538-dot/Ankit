<!DOCTYPE html>
<html>
<head>
  <title>Valentine</title>
  <style>
    body {
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      background: #ffb6c1;
      font-family: Arial, sans-serif;
    }
    .box {
      background: white;
      padding: 30px;
      border-radius: 15px;
      text-align: center;
      box-shadow: 0 10px 25px rgba(0,0,0,0.2);
    }
    h1 {
      margin-bottom: 20px;
    }
    button {
      padding: 12px 25px;
      font-size: 18px;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      margin: 10px;
    }
    #yes {
      background: #ff4d6d;
      color: white;
    }
    #no {
      position: absolute;
      background: #ccc;
    }
  </style>
</head>
<body>

<div class="box">
  <h1>Swati, will you be my Valentine? 💖</h1>
  <button id="yes" onclick="alert('Yay! 💕 I knew it 😍')">YES</button>
  <button id="no">NO</button>
</div>

<script>
  const noBtn = document.getElementById("no");
  noBtn.addEventListener("mouseover", () => {
    const x = Math.random() * (window.innerWidth - 100);
    const y = Math.random() * (window.innerHeight - 50);
    noBtn.style.left = x + "px";
    noBtn.style.top = y + "px";
  });
</script>

</body>
</html>
