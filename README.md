# CINEPLAY-TV-SUA-TV-ONLINE
Cineplay TV - Filmes, séries e canais ao vivo em um só lugar

<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Cineplay TV</title>

<style>
*{margin:0;padding:0;box-sizing:border-box}
body{
font-family:Arial;
color:#fff;
text-align:center;
background: linear-gradient(180deg,#0b0b0b,#1a0033);
overflow-x:hidden;
}

/* fundo animado */
body::before{
content:"";
position:fixed;
width:100%;
height:100%;
background: radial-gradient(circle at 20% 30%, rgba(123,44,255,0.3), transparent),
            radial-gradient(circle at 80% 70%, rgba(255,0,100,0.3), transparent);
z-index:-1;
animation:moverBg 12s infinite alternate;
}

@keyframes moverBg{
0%{transform:translate(0,0)}
100%{transform:translate(-40px,-40px)}
}

/* header */
.header{
background: linear-gradient(90deg,#7b2cff,#ff0066);
padding:15px;
font-weight:bold;
}

/* banner */
.banner{padding:60px 15px}

.overlay{
background:rgba(0,0,0,0.75);
padding:25px;
border-radius:12px;
}

/* botão */
.btn{
display:block;
margin:12px auto;
padding:15px;
background: linear-gradient(45deg,#ff2d2d,#ff0066);
color:#fff;
text-decoration:none;
border-radius:12px;
max-width:320px;
font-weight:bold;
box-shadow:0 0 15px rgba(255,0,100,0.6);
transition:0.3s;
}

.btn:hover{
transform:scale(1.08);
box-shadow:0 0 25px rgba(255,0,100,1);
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

.card:hover{transform:scale(1.05)}

.highlight{
border:2px solid #7b2cff;
box-shadow:0 0 15px #7b2cff;
}

.price{
font-size:22px;
color:#7b2cff;
margin:10px 0;
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
box-shadow:0 0 10px rgba(0,0,0,0.5);
animation:fadeIn 0.5s;
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

/* animações */
@keyframes fadeIn{
from{opacity:0;transform:translateY(10px)}
to{opacity:1;transform:translateY(0)}
}

</style>
</head>

<body>

<div class="header">
🔥 OFERTA TERMINA EM <span id="timer">10:00</span>
<p style="color:red;">⚠️ Poucas vagas disponíveis</p>
</div>

<div class="banner">
<div class="overlay">

<h1>🎬 Cineplay TV</h1>

<h2 style="color:#ff4444;">
🔥 Cancele Netflix e pague mais barato
</h2>

<p>
🎬 +100 MIL conteúdos<br>
📺 Canais ao vivo + Premiere<br>
⚡ Sem travar | HD/FULL HD
</p>

<a class="btn" href="https://wa.me/5582996062108?text=Quero%20teste">
🔥 TESTE GRÁTIS
</a>

<p style="color:#00ff88;font-weight:bold;">
🚀 Liberação imediata
</p>

<p style="color:#00ff88;">
👥 <span id="online">8</span> pessoas online
</p>

<img src="https://i.postimg.cc/SsXBVsR2/Screenshot-20260406-193310-IBO-REVENDA.jpg"
style="width:200px;border-radius:15px;margin-top:20px;">

</div>
</div>

<h2>💰 Pagamento Pix</h2>

<div class="card">
<p><b id="pix">3c3a8735-4475-4340-8090-649f95432cfa</b></p>

<button class="btn" onclick="copiarPix()">📋 Copiar Pix</button>

<a class="btn" href="https://wa.me/5582996062108?text=Já paguei">
📲 Enviar comprovante
</a>
</div>

<h2>💰 Planos</h2>

<div class="card">
<h3>1 Tela</h3>
<div class="price">R$ 24,90</div>
<a class="btn" href="#">Assinar</a>
</div>

<div class="card highlight">
<h3>2 Telas ⭐</h3>
<div class="price">R$ 34,90</div>
<a class="btn" href="#">Assinar</a>
</div>

<div class="card">
<h3>3 Telas</h3>
<div class="price">R$ 39,90</div>
<a class="btn" href="#">Assinar</a>
</div>

<a class="whatsapp-float" href="https://wa.me/5582996062108">💬</a>

<div class="popup" id="popup"></div>

<script>

// copiar pix
function copiarPix(){
let pix = document.getElementById("pix").innerText;

navigator.clipboard.writeText(pix)
.then(()=>alert("Pix copiado!"))
.catch(()=>alert("Erro ao copiar"));
}

// timer
let tempo = 600;

setInterval(()=>{
let m = Math.floor(tempo/60);
let s = tempo%60;

document.getElementById("timer").innerHTML =
m+":"+(s<10?"0"+s:s);

tempo--;

if(tempo <= 0) tempo = 600;

},1000);

// online fake
setInterval(()=>{
document.getElementById("online").innerHTML =
Math.floor(Math.random()*20)+5;
},3000);

// popup fake
const nomes = ["João","Maria","Carlos","Ana","Pedro","Lucas"];

setInterval(()=>{
let popup = document.getElementById("popup");

popup.innerHTML = "💰 "+nomes[Math.floor(Math.random()*nomes.length)]+" acabou de assinar";

popup.style.display="block";

setTimeout(()=>{
popup.style.display="none";
},3000);

},8000);

</script>

</body>
</html>
