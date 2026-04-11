<html lang="pt-br">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Cineplay TV</title>

<style>
*{margin:0;padding:0;box-sizing:border-box;max-width:100%}
html,body{overflow-x:hidden;font-family:Arial;background:#0b0b0b;color:#fff;text-align:center}

.header{background:#7b2cff;padding:12px;font-weight:bold}

.banner{
background:url('https://images.unsplash.com/photo-1524985069026-dd778a71c7b4?q=80&w=1200&auto=format&fit=crop') center/cover no-repeat;
padding:70px 20px;
}

.overlay{background:rgba(0,0,0,0.7);padding:30px;border-radius:10px}

.container{padding:20px}

.btn{
display:block;margin:12px auto;padding:15px;background:#ff2d2d;color:#fff;
text-decoration:none;border-radius:12px;width:90%;max-width:320px;
font-weight:bold;animation:pulsar 1.5s infinite;
}

.card{background:#1a1a1a;margin:15px auto;padding:20px;border-radius:15px;max-width:350px}

.highlight{border:2px solid #7b2cff}

.price{font-size:22px;color:#7b2cff;margin:10px 0}

.review{
background:#111;padding:15px;margin:10px auto;border-radius:10px;
max-width:320px;display:flex;align-items:center;gap:10px
}

.review img{width:40px;height:40px;border-radius:50%}

.footer{margin-top:30px;padding:20px;font-size:14px;color:#aaa}

.popup{
position:fixed;bottom:10px;left:10px;background:#111;padding:10px 15px;
border-radius:10px;font-size:13px;display:none
}

.whatsapp-float{
position:fixed;
bottom:20px;
right:20px;
text-decoration:none;
}

.instagram-float{
position:fixed;
bottom:110px;
right:20px;
text-decoration:none;
}

@keyframes flutuar{
0%{transform:translateY(0)}
50%{transform:translateY(-10px)}
100%{transform:translateY(0)}
}

@keyframes pulsar{
0%{transform:scale(1)}
50%{transform:scale(1.08)}
100%{transform:scale(1)}
}

@keyframes brilho{
0%{opacity:0.6}
50%{opacity:1}
100%{opacity:0.6}
}
</style>
</head>

<body>

<div class="header">
🔥 OFERTA LIMITADA TERMINA EM <span id="timer"></span>
<p style="color:red;">⚠️ Restam poucas vagas hoje</p>
</div>

<div class="banner">
<div class="overlay">

<img src="https://i.postimg.cc/8cS7DbFT/1000392886-removebg-preview.png" style="width:180px;background:transparent;">

<h2 style="color:#ff4444;">
🔥 Cancele Netflix, Prime e outros e pague muito mais barato
</h2>

<p>
🎬 +100 MIL conteúdos liberados<br>
📺 Canais ao vivo + Premiere + Telecine<br>
⚡ Sem travar | HD/FULL HD
</p>

<a class="btn" href="https://wa.me/5582996062108?text=Quero%20teste%20gratis%20agora">
🔥 TESTE GRÁTIS AGORA
</a>

<p style="color:#ff4444;font-weight:bold;">
⚠️ Restam apenas <span id="testes">10</span> testes grátis disponíveis
</p>

<a class="btn" href="https://aftv.news/1072646">
<img src="https://i.postimg.cc/63sGqhDZ/file-00000000d004720e80be58868406bf64.png" style="width:40px;vertical-align:middle;margin-right:8px;">
📲 BAIXAR APLICATIVO
</a>

<!-- VIDEO ADICIONADO -->
<div style="margin-top:20px;">
<iframe width="100%" height="220"
src="https://www.youtube.com/embed/K3QLrvM39fw"
frameborder="0"
allowfullscreen
style="border-radius:10px;">
</iframe>
</div>

<p style="font-size:13px;color:#aaa;">
⚠️ Use no app Downloader (TV Box / Fire Stick)
</p>

<p style="color:#00ff88;font-weight:bold;">
🚀 Acesso liberado em poucos minutos<br>
👥 <span id="online">12</span> pessoas vendo agora
</p>

<div style="margin-top:30px;">
<div style="display:inline-block;background:#111;padding:10px;border-radius:30px;box-shadow:0 0 20px rgba(0,0,0,0.5);animation: flutuar 3s infinite;">
<img src="https://i.postimg.cc/SsXBVsR2/Screenshot-20260406-193310-IBO-REVENDA.jpg"
style="width:220px;border-radius:20px;animation: brilho 2s infinite;">
</div>
</div>

</div>
</div>

<div class="container">

<h2>⭐ Avaliações Reais</h2>

<div class="review">
<img src="https://randomuser.me/api/portraits/men/32.jpg">
<p>Top demais, sem travar</p>
</div>

<div class="review">
<img src="https://randomuser.me/api/portraits/women/45.jpg">
<p>Melhor que Netflix</p>
</div>

<h2>💰 Pagamento via Pix</h2>

<p>⚡ Liberação rápida após envio do comprovante</p>

<div style="background:#111;padding:15px;border-radius:10px;margin:15px;">
<p><b>3c3a8735-4475-4340-8090-649f95432cfa</b></p>

<button class="btn" onclick="copiarPix()">📋 Copiar chave Pix</button>

<a class="btn" href="https://wa.me/5582996062108?text=Já%20fiz%20o%20pagamento%20via%20Pix">
📲 Enviar comprovante
</a>

<p style="color:#7b2cff;">🔒 Pagamento seguro</p>
</div>

<!-- resto do site permanece igual -->

<div class="footer">© Cineplay TV</div>

<a class="whatsapp-float" href="https://wa.me/5582996062108">
<img src="https://upload.wikimedia.org/wikipedia/commons/6/6b/WhatsApp.svg" style="width:40px;height:40px;">
</a>

<a class="instagram-float" href="https://www.instagram.com/cineplayofc64" target="_blank">
<img src="https://upload.wikimedia.org/wikipedia/commons/a/a5/Instagram_icon.png" style="width:40px;height:40px;">
</a>

<div class="popup" id="popup"></div>

<script>

function copiarPix(){
navigator.clipboard.writeText("3c3a8735-4475-4340-8090-649f95432cfa");
alert("Chave Pix copiada!");
}

// TIMER
let time=600;
setInterval(()=>{
let m=Math.floor(time/60);
let s=time%60;
document.getElementById('timer').innerHTML=m+":"+(s<10?'0':'')+s;
time--;
if(time<0) time=600;
},1000);

// POPUP
const nomes=[
"João - SP","Maria - RJ","Carlos - MG","Ana - BA",
"Pedro - CE","Lucas - PE","Fernanda - PR"
];

setInterval(()=>{
let popup=document.getElementById("popup");
let nome=nomes[Math.floor(Math.random()*nomes.length)];
popup.innerHTML=nome+" acabou de ativar o teste grátis 🔥";
popup.style.display="block";

setTimeout(()=>{
popup.style.display="none";
},3000);

},8000);

// CONTADOR ONLINE
setInterval(()=>{
document.getElementById("online").innerHTML = Math.floor(Math.random()*10)+10;
},3000);

// CONTADOR TESTES
let testes = 10;
setInterval(()=>{
if(testes > 3){
testes--;
document.getElementById("testes").innerHTML = testes;
}
},30000);

</script>

</body>
</html>
