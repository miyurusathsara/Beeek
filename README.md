<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Auto-Open Box After 3 Seconds</title>
  <style>
    body {
      font-family: sans-serif;
      padding: 40px;
      background-color: #f0f0f0;
    }

    .large-text {
      font-size: 1.5em;
      line-height: 1.6;
      color: #333;
      margin-bottom: 30px;
    }

    .btn {
      padding: 10px 20px;
      font-size: 16px;
      cursor: pointer;
      background-color: #007BFF;
      color: white;
      border: none;
      border-radius: 4px;
    }

    .modal {
      display: none; /* Hidden by default */
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background-color: rgba(0, 0, 0, 0.5); /* Overlay */
      justify-content: center;
      align-items: center;
    }

    .modal-box {
      background-color: white;
      padding: 50px 90px;
      border-radius: 8px;
      max-width: 500px;
      text-align: center;
    }

    .close-btn {
      margin-top: 20px;
      background-color: #dc3545;
    }
  </style>
</head>
<body>

  <div class="large-text">
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur in consequat tortor, a tincidunt metus. Duis pharetra augue nec quam scelerisque, a commodo sssssssssnibh scelerisque. Mauris non feugiat turpis, ut varius purus. Suspendisse ut Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur in consequat tortor, a tincidunt metus. Duis pharetra Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur in consequat tortor, a tincidunt metus. Duis pharetra augue nec quam scelerisque, a commodo sssssssssnibh scelerisque. Mauris non feugiat turpis, ut varius purus. Suspendisse ut posuere est. Sed at dui lorem.  nec quam scelerisque, a commodo sssssssssnibh scelerisque. Mauris non feugiat turpis, ut varius purus. Suspendisse ut posuere est. Sed at dui lorem.  est. Sed Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur in consequat tortor, a tincidunt metus. Duis pharetra augue nec quam scelerisque, a commodo sssssssssnibh scelerisque. Mauris non feugiat turpis, ut varius purus. Suspendisse ut posuere est. Sed at dui lorem.  dui lorem. Integer sed diam imperdiet, finibus justo sed, tincidunt nunc.
  </div>

  <button class="btn" onclick="openBox()">Click to Open Box</button>

  <!-- Modal Box -->
  <div id="myModal" class="modal">
    <div class="modal-box">
      <h2>This is a Box!</h2>
      <p>You opened Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur in consequat tortor, a tincidunt metus. Duis Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur in consequat tortor, a tincidunt metus. Duis pharetra Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur in consequat tortor, a tincidunt metus. Duis pharetra augue nec quam scelerisque, a commodo sssssssssnibh scelerisque. Mauris non feugiat turpis, ut varius purus. Suspendisse ut posuere est. Sed at dui lorem.  nec quam scelerisque, a commodo sssssssssnibh scelerisque. Mauris non feugiat turpis, ut varius purus. Suspendisse ut posuere est. Sed at dui lorem.  augue nec quam scelerisque, a commodo sssssssssnibh scelerisque. Mauris non feugiat turpis, ut varius purus. Suspendisse ut posuere est. Sed at dui lorem.  automatically after 3 seconds.</p>
      <button class="btn close-btn" onclick="closeBox()">Close</button>
    </div>
  </div>

  <script>
    function openBox() {
      document.getElementById('myModal').style.display = 'flex';
    }

    function closeBox() {
      document.getElementById('myModal').style.display = 'none';
    }

    // Automatically open the box after 3 seconds
    window.onload = function() {
      setTimeout(openBox, 5000); // 3000 ms = 3 seconds
    };
  </script>

</body>
</html>
