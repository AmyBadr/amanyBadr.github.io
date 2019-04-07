# Machine Learning - Fashion Mnist Assignment # 3
Amany Said Badr El-Din


<html lang="en">
<head>
<meta charset="UTF-8" />
<title>Fashion Mnist Recognition</title>

<!-- bs4 css -->
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.1.0/css/bootstrap.min.css"/>
	
<!-- css pie -->
<link rel="stylesheet" href="pie.css">

<!-- jQuery library -->
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>

<!-- Popper JS -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.0/umd/popper.min.js"></script>

<!-- Latest compiled JavaScript -->
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.1.0/js/bootstrap.min.js"></script>

<!-- TensorFlow.js script -->
<script src="https://cdn.jsdelivr.net/npm/@tensorflow/tfjs@latest"> </script>
<!-- <script src="https://cdnjs.cloudflare.com/ajax/libs/tensorflow/1.0.3/tf.min.js"></script> -->
<!-- canvas script -->
<script src="fabric.js"></script>
	
<!-- main script -->
<script src = "main.js" > </script>

<!-- main css -->
<link rel = "stylesheet" href="main.css" > 
	
</head>
<body>
<nav class="navbar navbar-expand-sm bg-light navbar-light">
  <!-- Brand/logo -->
  <a class="navbar-brand" href="#"><h1>FashionMnist<small>Recognition</small></h1></a>
  </nav>
<div class="container-fluid"> 

<blockquote class="blockquote text-justify" style="margin:30px;">
 <p> This App is a simple tool that uses CNN to recognize drawings. 
 The CNN was trained to recognize 100 classes using the quick draw dataset. The accuracy could be improved
but I focused on making the model light. The table  will show the top 5 predictions. </p>
    <footer class="blockquote-footer">Fashion Mnist</footer>
  </blockquote>
</div>

<div class="row">
  <div class="col" style ='margin-left:100px;'>
<h4 id ='status' >Loading Model... </h4>	  
<canvas id="canvas" width="300" height="300" class="canvas" style="border:1px solid #b9bfc9;margin-top:25px;"></canvas>
<div class="btn-group" style = 'margin-top:40px; '>
<input type="range" min="5" max="20" value="10" class="slider" id="myRange" style ='margin-top:20px;'>
<button type="button" class="btn btn-outline-primary" onclick ='erase()' style ='margin-left:10px;' disabled>Clear</button>
    </div>   
</div>
  <div class="col">
    <section style="margin-top:120px">
    <div class="pieID pie">
      
    </div>
    <ul class="pieID legend">
      <li>
        <em id = "sym1"></em>
        <span id = "prob1" ></span>
      </li>
      <li>
        <em id = "sym2"></em>
        <span id = "prob2"></span>
      </li>
      <li>
        <em id = "sym3"></em>
        <span id = "prob3"></span>
      </li>
      <li>
        <em id = "sym4"></em>
        <span id = "prob4"></span>
      </li>
      <li>
        <em id = "sym5"></em>
        <span id = "prob5"></span>
      </li>
    </ul>
  </section>
</div>
</div>  
</body>
<script src="pie.js"></script>
<script>
	console.log('starting');
	start('en')
</script>
</html>


