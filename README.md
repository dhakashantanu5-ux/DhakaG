# DhakaG
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>For Nainuu ❤️</title>

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Poppins,sans-serif;
}

body{
height:100vh;
overflow:hidden;
display:flex;
justify-content:center;
align-items:center;
background:linear-gradient(135deg,#ff5f9e,#ff9a3d);
color:white;
}

.container{
text-align:center;
padding:20px;
max-width:600px;
}

h1{
font-size:55px;
margin-bottom:15px;
}

h2{
font-size:40px;
margin-bottom:20px;
}

p{
font-size:20px;
margin-bottom:25px;
}

.buttons{
position:relative;
height:120px;
}

button{
padding:15px 40px;
border:none;
border-radius:40px;
font-size:22px;
cursor:pointer;
transition:.3s;
}

#yesBtn{
background:white;
color:#ff4b7d;
font-weight:bold;
}

#yesBtn:hover{
transform:scale(1.1);
}

#noBtn{
position:absolute;
left:65%;
background:#ffffff33;
color:white;
backdrop-filter:blur(10px);
}

#page2{
display:none;
text-align:center;
animation:fade .8s;
}

img{
width:260px;
border-radius:20px;
margin-top:20px;
box-shadow:0 0 20px rgba(255,255,255,.4);
}

@keyframes fade{
from{opacity:0;}
to{opacity:1;}
}

.heart{
position:absolute;
color:white;
font-size:25px;
animation:float 5s linear infinite;
}

@keyframes float{
0%{
transform:translateY(100vh);
opacity:1;
}
100%{
transform:translateY(-100px);
opacity:0;
}
}
</style>
</head>

<body>

<div class="container" id="page1">

<p>From: <b>Shntnu ❤️</b></p>

<h1>Will you forever be mine?</h1>

<h2>Nainuu 🫶💝</h2>

<p>Babyyyyy, loveeee youuuu coohhh</p>

<div class="buttons">

<button id="yesBtn">Yes ❤️</button>

<button id="noBtn">No 😈</button>

</div>

</div>

<div class="container" id="page2">

<h1>Yay! I knew you'd say YES! ❤️</h1>

<p>You're the most amazing person I know.<br>
I love you endlessly.<br><br>

<b>— Shntnu ❤️</b>
</p>

<img src="https://media.tenor.com/6vPS-4kM6QMAAAAC/cute-cat.gif">

<p style="margin-top:20px;">🤍 You just made me the happiest!</p>

</div>

<script>

const no=document.getElementById("noBtn");

no.addEventListener("mouseover",()=>{

let x=Math.random()*(window.innerWidth-120);

let y=Math.random()*(window.innerHeight-80);

no.style.left=x+"px";
no.style.top=y+"px";

});

document.getElementById("yesBtn").onclick=()=>{

document.getElementById("page1").style.display="none";

document.getElementById("page2").style.display="block";

createHearts();

};

function createHearts(){

setInterval(()=>{

let h=document.createElement("div");

h.className="heart";

h.innerHTML="❤️";

h.style.left=Math.random()*100+"vw";

h.style.fontSize=(20+Math.random()*30)+"px";

document.body.appendChild(h);

setTimeout(()=>h.remove(),5000);

},200);

}

</script>

</body>
</html>
