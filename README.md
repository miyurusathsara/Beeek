<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Button Click Box</title>
  <style>
    #box {
      width: 100px;
      height: 100px;
      background-color: lightblue;
      display: none; /* Hidden by default */
      margin-top: 10px;
    }
  </style>
</head>
<body>

  <button onclick="showBox()">Click Me</button>

  <div id="box"></div>

  <script>
    function showBox() {
      document.getElementById("box").style.display = "block";
    }
  </script>

</body>
</html>
