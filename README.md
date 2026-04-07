# CINEPLAY-TV-SUA-TV-ONLINE
Cineplay TV - Filmes, séries e canais ao vivo em um só lugar

 <!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Cineplay TV</title>

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
}

html{
scroll-behavior:smooth;
}

body{
font-family:Arial;
color:#fff;
text-align:center;
background: linear-gradient(180deg,#0b0b0b,#1a0033);
overflow-x:hidden;
}

/* fundo animado leve */
body::before{
content:"";
position:fixed;
width:100%;
height:100%;
background: radial-gradient(circle at 20% 30%, rgba(123,44,255,0.2), transparent),
            radial-gradient(circle at 80% 70%, rgba(255,0,100,0.2), transparent);
z-index:-1;
}

/* header */
.header{
background: linear-gradient(90deg,#7b2cff,#ff0066);
padding:14px;
font-weight:bold;
}

/* banner */
.banner{
padding:50px 15px;
}

.overlay{
background:rgba(0,0,0,0.7);
padding:20px;
border-radius:12px;
}

/* botão melhorado */
.btn{
display:block;
margin:12px auto;
padding:16px;
background: linear-gradient(45deg,#ff2d2d,#ff0066);
color:#fff;
text-decoration:none;
border-radius:12px;
width:90%;
max-width:320px;
font-weight:bold;
box-shadow:0 5px 20px rgba(255,0,100,0.5);
transition:0.2s;
}

.btn:active{
transform:scale(0.95);
}

/* cards */
.card{
background:#111;
margin:15px auto;
padding:20px;
border-radius:15px;
max-width:350px;
transition:0.3s;
}

.card:hover{
transform:scale(1.03);
}

.highlight{
border:2px solid #7b2cff;
box-shadow:0 0 15px #7b2cff;
}

.price{
font-size:22px;
color:#7b2cff;
margin:10px 0;
}

/* imagem */
img{
width:100%;
max-width:220px;
border-radius:15px;
margin-top:20px;
}

/* animação scroll */
.fade{
opacity:0;
transform:translateY(20px);
transition:1s;
}

.fade.show{
opacity:1;
transform:translateY(0);
}

/* popup */
.popup{
position:fixed;
bottom:20px;
left:20px;
background:#000;
padding:12px 18px;
border-radius:10px;
font-size:13px;
display:none;
}

/* whatsapp */
.whatsapp-float{
position:fixed;
bottom:20px;
right:20px;
background:#25D366;
padding:15px;
border-radius:50%;
font-size:22px;
text-decoration:none;
}

</style>
</head>

<body>

<div class="header">
🔥 OFERTA TERMINA EM <span id="timer">10:00</span>
</div>

<div class="banner fade">
<div class="overlay">

<h1>🎬 Cineplay TV</h1>

<h2 style="color:#ff4444;">
🔥 Pague muito mais barato que streaming
</h2>

<p>
🎬 +100 MIL conteúdos<br>
📺 Canais ao vivo<br>
⚡ Sem travar | HD/FULL HD
</p>

<a class="btn" href="https://wa.me/5582996062108">🔥 TESTE GRÁTIS</a>

<p style="color:#00ff88;">
👥 <span id="online">8</span> online agora
</p>

<img src="https://i.postimg.cc/SsXBVsR2/Screenshot-20260406-193310-IBO-REVENDA.jpg">

</div>
</div>

<h2 class="fade">💰 Pagamento Pix</h2>

<div class="card fade">
<p><b id="pix">3c3a8735-4475-4340-8090-649f95432cfa</b></p>

<button class="btn" onclick="copiarPix()">📋 Copiar Pix</button>
</div>

<h2 class="fade">💰 Planos</h2>

<div class="card fade">
<h3>1 Tela</h3>
<div class="price">R$ 24,90</div>
<a class="btn" href="#">Assinar</a>
</div>

<div class="card highlight fade">
<h3>2 Telas ⭐</h3>
<div class="price">R$ 34,90</div>
<a class="btn" href="#">Assinar</a>
</div>

<div class="card fade">
<h3>3 Telas</h3>
<div class="price">R$ 39,90</div>
<a class="btn" href="#">Assinar</a>
</div>

<a class="whatsapp-float" href="https://wa.me/5582996062108">💬</a>

<div class="popup" id="popup"></div>

<script>

// animação ao rolar
const fades = document.querySelectorAll('.fade');

function aparecer(){
fades.forEach(el=>{
const top = el.getBoundingClientRect().top;
if(top < window.innerHeight - 50){
el.classList.add('show');
}
});
}

window.addEventListener('scroll', aparecer);
aparecer();

// copiar pix
function copiarPix(){
let pix = document.getElementById("pix").innerText;
navigator.clipboard.writeText(pix);
alert("Pix copiado!");
}

// timer
let tempo = 600;
setInterval(()=>{
let m = Math.floor(tempo/60);
let s = tempo%60;
document.getElementById("timer").innerHTML =
m+":"+(s<10?"0"+s:s);
tempo--;
if(tempo<=0) tempo=600;
},1000);

// online fake
setInterval(()=>{
document.getElementById("online").innerHTML =
Math.floor(Math.random()*20)+5;
},3000);

// popup fake
const nomes=["João","Maria","Carlos","Ana"];
setInterval(()=>{
let popup=document.getElementById("popup");
popup.innerHTML="💰 "+nomes[Math.floor(Math.random()*nomes.length)]+" assinou!";
popup.style.display="block";
setTimeout(()=>popup.style.display="none",3000);
},8000);

</script>

</body>
</html>
