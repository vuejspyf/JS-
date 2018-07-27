
 <!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8" />
    
    <title>Page Title</title>
   <script>
   function toDou(n){
if(n<10){
    return '0'+n;

}
else{
    return''+n;
}   }
 window.onload=function(){
var aImg=document.getElementsByTagName('img');
function tick(){
var oDate=new Date();
var str=toDou(oDate.getHours())+toDou(oDate.getMinutes())+toDou(oDate.getSeconds());
for(var i=0;i<aImg.length;i++)
{
    aImg[i].src='img/'+str.charAt(i)+'.png';
}
}
setInterval(tick,1000);
tick();

 }  ;
   </script>
</head>
<body style="background:black;color:white;margin:350px;
font-size:50px;">
    <img src="img/0.png"/>
    <img src="img/0.png"/>
    :
    <img src="img/0.png"/>
    <img src="img/0.png"/>
    :
    <img src="img/0.png"/>
    <img src="img/0.png"/>
</body>
</html>
