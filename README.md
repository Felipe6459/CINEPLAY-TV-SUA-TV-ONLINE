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

html,body{
overflow-x:hidden;
font-family:Arial;
background:#0b0b0b;
color:#fff;
text-align:center;
}

/* CORREÇÃO DO VAZAMENTO */
.banner{
background:url('https://images.unsplash.com/photo-1524985069026-dd778a71c7b4?q=80&w=1200&auto=format&fit=crop');
background-size:cover;
background-position:center;
padding:60px 15px;
max-width:100%;
overflow:hidden;
}

/* imagens seguras */
img{
max-width:100%;
height:auto;
display:block;
margin:auto;
}

.header{
background:#7b2cff;
padding:12px;
font-weight:bold;
}

.overlay{
background:rgba(0,0,0,0.7);
padding:20px;
border-radius:10px;
}

.container{
padding:15px;
}

.btn{
display:block;
margin:12px auto;
padding:15px;
background:#ff2d2d;
color:#fff;
text-decoration:none;
border-radius:12px;
width:90%;
max-width:320px;
font-weight:bold;
}

.card{
background:#1a1a1a;
margin:15px auto;
padding:20px;
border-radius:15px;
max-width:350px;
}

.highlight{
border:2px solid #7b2cff;
}

.price{
font-size:22px;
color:#7b2cff;
margin:10px 0;
}

.review{
background:#111;
padding:12px;
margin:10px auto;
border-radius:10px;
max-width:320px;
display:flex;
align-items:center;
gap:10px;
}

.review img{
width:40px;
height:40px;
border-radius:50%;
}

.popup{
position:fixed;
bottom:10px;
left:10px;
background:#111;
padding:10px 15px;
border-radius:10px;
font-size:13px;
display:none;
}

.whatsapp-float{
position:fixed;
bottom:20px;
right:20px;
background:#25D366;
color:#fff;
padding:15px;
border-radius:50%;
font-size:22px;
text-decoration:none;
}

.footer{
margin-top:30px;
padding:20px;
font-size:14px;
color:#aaa;
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

<h1>🎬 Cineplay TV</h1>

<h2 style="color:#ff4444;">
🔥 Cancele Netflix e pague mais barato
</h2>

<p>
🎬 +100 MIL conteúdos<br>
📺 Canais ao vivo<br>
⚡ Sem travar
</p>

<a class="btn" href="https://wa.me/5582996062108">
🔥 TESTE GRÁTIS AGORA
</a>

<!-- ✅ BOTÃO INSTAGRAM (AGORA FUNCIONANDO) -->
<a class="btn" href="https://www.instagram.com/cineplayofc64" target="_blank">
📸 Siga a gente no Instagram 🔥
</a>

<p style="color:#00ff88;">
🚀 Liberação imediata
</p>

<img src="https://i.postimg.cc/SsXBVsR2/Screenshot-20260406-193310-IBO-REVENDA.jpg">

</div>
</div>

<div class="container">

<h2>⭐ Avaliações</h2>

<div class="review">
<img src="https://randomuser.me/api/portraits/men/32.jpg">
<p>Top demais</p>
</div>

<div class="review">
<img src="https://randomuser.me/api/portraits/women/45.jpg">
<p>Muito bom</p>
</div>

</div>

<a class="whatsapp-float" href="https://wa.me/5582996062108">💬</a>

<script>
let time=600;
setInterval(()=>{
let m=Math.floor(time/60);
let s=time%60;
document.getElementById('timer').innerHTML=m+":"+(s<10?'0':'')+s;
time--;
if(time<0) time=600;
},1000);
</script>

</body>
</html>
