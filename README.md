<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>Sorry</title>
  <style>
    body{
      background:black;
      color:white;
      font-family:Arial;
      padding:20px;
    }
    #text{
      white-space:pre-wrap;
      font-size:18px;
    }
  </style>
</head>
<body>
  <div id="text"></div>

<script>
let t = document.getElementById("text");
let i = 1;
let max = 1000;

function writeSorry(){
  if(i <= max){
    t.textContent += i + ". Sorry\n";
    i++;
    window.scrollTo(0, document.body.scrollHeight);
    setTimeout(writeSorry, 10);
  }
}
writeSorry();
</script>
</body>
</html>
