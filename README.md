<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Animation3</title>
  <style type="text/css">
    .flexcontainer{
  margin: 30px auto;
  max-width: 700px;/*
  width: 500px;*/
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
}


.box{
  width: 150px;
  margin: 20px;
  background: lightgray;
  /*cursor: pointer;*/
  color: white;
  text-align: center;
  line-height: 130px;
}


.blue{
  background-color: skyblue;
  opacity: 0.5;
}


.scaleX{
  transform: scaleX(1);
  transition: transform 0.5s ease;
}


.box:hover .scaleX{
  transform: scaleX(1.5);
}

.scaleY{
  transform: scaleY(1);
  transition: transform 0.5s ease;
}


.box:hover .scaleY{
  transform: scaleY(1.5);
}

.scale{
  transform: scale(1, 1);
  transition: transform 0.5s ease;
}


.box:hover .scale{
  transform: scale(1.5, 1.5);
}

.translateX{
  transform: translateX(1);
  transition: transform 0.5s ease;
}


.box:hover .translateX{
  transform: translateX(20px);
}

.translateY{
  transform: translateY(1);
  transition: transform 0.5s ease;
}


.box:hover .translateY{
  transform: translateY(20px);
}

.translate{
  transform: translate(1,1);
  transition: transform 0.5s ease;
}


.box:hover .translate{
  transform: translate(20px, 20px);
}

.matrix{
  transform: matrix(1, 1, 1, 1);
  transition: transform 0.5s ease;  
}

.box:hover .matrix{
    transform: matrix(1, -1, 0, 1, 0, 0); /* matrix(scaleX(), skewY(), skewX(), scaleY(), translateX(), translateY()) Standard syntax */
}

.rotate{
  transform: rotate(0);
  transition: transform 0.5s ease;  
}

.box:hover .rotate{
    transform: rotate(270deg); /* Standard syntax */
}

.skew{
  transform: skew(1, 1);
  transition: transform 0.5s ease;  
}

.box:hover .skew{
    transform: skew(30deg, 20deg);
 /* Standard syntax */
}

.skewX{
  transform: skewX(1);
  transition: transform 0.5s ease;  
}

.box:hover .skewX{
    transform: skewX(30deg);
 /* Standard syntax */
}

.skewY{
  transform: skewY(1);
  transition: transform 0.5s ease;  
}

.box:hover .skewY{
    transform: skewY(30deg);
 /* Standard syntax */
}

/*.matrix3d{
  transform: matrix3d(1);
  transition: transform 0.5s ease;  
}

.box:hover .matrix3d{
transform: matrix3d(0.8535533905932737, 0.4999999999999999, 0.14644660940672619, 0, -0.4999999999999999, 0.7071067811865476, 0.4999999999999999, 0, 0.14644660940672619, -0.4999999999999999, 0.8535533905932737, 0, 22.62994231491119, -20.3223304703363, 101.3700576850888, 1)
 /* Standard syntax */
}
/*
.translate3d{
  transform: translate3d(1px, 1px, 1);
  transition: transform 0.5s ease;  
}

.box:hover .translate3d{
  transform: translate3d(1px, 1px, 50px) rotate3d(3, 2, 2, 90deg);
 /* Standard syntax */
}

.rotateY{
  transform: perspective(1) scaleZ(1) rotateY(0deg);
  transition: transform 0.5s ease; 
/*   perspective: 300px; */
/*   transform-style: preserve-3d; */
}

.box:hover .rotateY{
/*   transform: translate3d(42px, 42px, 42px); */
  transform: perspective(500px) scaleZ(2) rotateY(45deg);
 /* Standard syntax */
}

.rotateX{
/*   perspective: 100px; */
  transform: perspective(1) scaleZ(1) rotateX(0deg);
  transition: transform 0.5s ease;  
}

.box:hover .rotateX{
  transform: perspective(500px) scaleZ(2) rotateX(45deg);
 /* Standard syntax */
}

/*.translateZ{
  transform: translateZ(1px);
  transition: transform 0.5s ease; 
}

.box:hover .translateZ{

  transform: rotate3d(3, 2, 2, 90deg) translateZ(50px);
 /* Standard syntax */
}*/


</style>
</head>
<body>
<div class="flexcontainer">
  <div class="box">
    <div class="blue scaleX ">
      scaleX
    </div>
  </div>
  <div class="box">
    <div class="blue scaleY">
      scaleY
    </div>
  </div> 
  <div class="box">
    <div class="blue scale">
      scale
    </div>
  </div> 
  <div class="box">
    <div class="blue translateX">
      translateX
    </div>
  </div> 
  <div class="box">
    <div class="blue translateY">
      translateY
    </div>
  </div>
  <div class="box">
    <div class="blue translate">
      translate
    </div>
  </div>  
  <div class="box">
    <div class="blue matrix">
      matrix
    </div>
  </div>  
  <div class="box">
    <div class="blue rotate">
      rotate
    </div>
  </div>  
  <div class="box">
    <div class="blue skew">
      skew
    </div>
  </div>
  <div class="box">
    <div class="blue skewX">
      skewX
    </div>
  </div>  
  <div class="box">
    <div class="blue skewY">
      skewY
    </div>
  </div>  
  <!-- <div class="box">
    <div class="blue matrix3d">
      matrix3d
    </div>
  </div>
  <div class="box">
    <div class="blue translate3d">
      translate3d
    </div>
  </div> -->
 <div class="box">
   <div class="blue rotateY">
    rotateY
   </div>
 </div>
 <div class="box">
   <div class="blue rotateX">
    rotateX
   </div>
 </div>
 <!-- <div class="box">
   <div class="blue translateZ">
    translateZ
   </div>
 </div>  -->
</div>
</body>
</html>
