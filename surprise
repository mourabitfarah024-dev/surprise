<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>For Sata ❤️</title>

<style>
body{
  margin:0;
  background:black;
  color:white;
  font-family:Arial;
  text-align:center;
  overflow:hidden;
}

#countdown{
  font-size:60px;
  margin-top:120px;
}

.cake{
  font-size:120px;
  cursor:pointer;
  display:none;
}

#heart{
  font-size:150px;
  display:none;
  animation:beat 1s infinite;
}

@keyframes beat{
  0%{transform:scale(1);}
  50%{transform:scale(1.2);}
  100%{transform:scale(1);}
}

#photo{
  width:180px;
  height:180px;
  border-radius:50%;
  position:absolute;
  left:50%;
  top:45%;
  transform:translate(-50%,-50%);
  display:none;
  border:4px solid white;
}

#message{
  margin-top:20px;
  font-size:24px;
  width:80%;
  margin-left:auto;
  margin-right:auto;
}

.fire{
  position:absolute;
  font-size:25px;
  animation:firework 1.5s forwards;
}

@keyframes firework{
  from{opacity:1;transform:translate(0,0);}
  to{opacity:0;transform:translate(var(--x),var(--y));}
}
</style>
</head>

<body>

<div id="countdown">3</div>

<div class="cake" onclick="startMagic()">🎂</div>

<div id="heart">❤️</div>

<img id="photo" src="PUT_IMAGE_HERE">

<div id="message"></div>

<audio id="music">
<source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3">
</audio>

<script>

let c=3;
let counter=setInterval(()=>{
  c--;
  document.getElementById("countdown").innerHTML=c;
  if(c==0){
    clearInterval(counter);
    document.getElementById("countdown").style.display="none";
    document.querySelector(".cake").style.display="block";
  }
},1000);

let text="Happy Birthday Sata ❤️\nYou are one of the most beautiful parts of my life.\nMay your days always shine with happiness and love ✨🎂";

let i=0;
function typeText(){
  if(i<text.length){
    document.getElementById("message").innerHTML+=text.charAt(i);
    i++;
    setTimeout(typeText,40);
  }
}

function fireworks(){
  for(let i=0;i<60;i++){
    let f=document.createElement("div");
    f.className="fire";
    f.innerHTML="✨";

    f.style.left=window.innerWidth/2+"px";
    f.style.top=window.innerHeight/2+"px";

    f.style.setProperty('--x',(Math.random()*800-400)+"px");
    f.style.setProperty('--y',(Math.random()*800-400)+"px");

    document.body.appendChild(f);
    setTimeout(()=>f.remove(),1500);
  }
}

function startMagic(){
  document.getElementById("music").play();
  document.querySelector(".cake").style.display="none";
  document.getElementById("heart").style.display="block";
  document.getElementById("photo").style.display="block";

  fireworks();
  typeText();
}

</script>

</body>
</html>
