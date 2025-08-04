<!DOCTYPE html>
<html>
<head>
  <title>Simulated New Body</title>
  <style>
    #newBody {
      width: 600px;
      height: 400px;
      border: 2px solid #000;
      margin: 50px auto;
      padding: 20px;
      background-color: #fff;
      display: none;
      box-shadow: 0 0 10px rgba(0,0,0,0.5);
    }
  </style>
</head>
<body>

  <button onclick="document.getElementById('newBody').style.display = 'block'">
    Show New Body
  </button>

  <div id="newBody">
    <h2>This is the new "body"</h2>
    <p>Custom width and height inside the same HTML body.</p>
  </div>

</body>
</html>
