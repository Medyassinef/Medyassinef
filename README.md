<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Your GitHub Profile</title>
</head>
<body>
  <div class="container">
    <div class="spinner"></div>
    <div class="moving-box"></div>
  </div>

  <script>
    const spinner = document.querySelector('.spinner');
    const movingBox = document.querySelector('.moving-box');

    function animateBox() {
      movingBox.style.transform = 'translateX(200px)';
      setTimeout(() => {
        movingBox.style.transform = 'translateX(0)';
        setTimeout(animateBox, 1000);
      }, 1000);
    }

    animateBox();
  </script>

  <style>
    .container {
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      background-color: #f0f0f0;
    }

    .spinner {
      width: 50px;
      height: 50px;
      background-color: #3498db;
      animation: spin 2s linear infinite;
      margin-right: 20px;
    }

    .moving-box {
      width: 50px;
      height: 50px;
      background-color: #e74c3c;
      transition: transform 1s ease;
    }

    @keyframes spin {
      0% { transform: rotate(0deg); }
      100% { transform: rotate(360deg); }
    }
  </style>
</body>
</html>

Feel free to explore my repositories, and don't forget to ⭐️ your favorite projects!
