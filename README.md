# CINEPLAY-TV-SUA-TV-ONLINE
Cineplay TV - Filmes, séries e canais ao vivo em um só lugar
<html
 <div style="background:#111;padding:15px;border-radius:10px;margin:15px;">
<p><b>3c3a8735-4475-4340-8090-649f95432cfa</b></p>

<button class="btn" onclick="copiarPix()">📋 Copiar chave Pix</button>

<a class="btn" href="https://wa.me/5582996062108?text=Já%20fiz%20o%20pagamento%20via%20Pix">
📲 Enviar comprovante
</a>

<p style="color:#7b2cff;">🔒 Pagamento seguro</p>
</div>

<h2>💰 Planos Mensais</h2>

<div class="card">
<h3>1 Tela</h3>
<div class="price">R$ 24,90</div>
<a class="btn" href="https://wa.me/5582996062108?text=Quero%201%20tela">Assinar</a>
</div>

<div class="card highlight">
<h3>2 Telas ⭐ Mais Vendido</h3>
<div class="price">R$ 34,90</div>
<a class="btn" href="https://wa.me/5582996062108?text=Quero%202%20telas">Assinar</a>
</div>

<div class="card">
<h3>3 Telas</h3>
<div class="price">R$ 39,90</div>
<a class="btn" href="https://wa.me/5582996062108?text=Quero%203%20telas">Assinar</a>
</div>

<h2>🔥 Planos Anuais</h2>

<div class="card">
<h3>1 Tela</h3>
<div class="price">R$ 179,90</div>
<a class="btn" href="https://wa.me/5582996062108?text=Quero%20anual%201%20tela">Assinar</a>
</div>

<div class="card highlight">
<h3>2 Telas ⭐ Melhor Custo</h3>
<div class="price">R$ 229,90</div>
<a class="btn" href="https://wa.me/5582996062108?text=Quero%20anual%202%20telas">Assinar</a>
</div>

<div class="card">
<h3>3 Telas</h3>
<div class="price">R$ 264,90</div>
<a class="btn" href="https://wa.me/5582996062108?text=Quero%20anual%203%20telas">Assinar</a>
</div>

<h2>📺 Compatibilidade</h2>
<p>
📱 Android<br>
📺 Smart TV<br>
📦 TV Box<br>
💻 Computador
</p>

</div>

<div class="footer">© Cineplay TV</div>

<a class="whatsapp-float" href="https://wa.me/5582996062108">💬</a>

<div class="popup" id="popup"></div>

<script>
function copiarPix(){
navigator.clipboard.writeText("3c3a8735-4475-4340-8090-649f95432cfa");
alert("Chave Pix copiada!");
}

let time=600;
setInterval(()=>{
let m=Math.floor(time/60);
let s=time%60;
document.getElementById('timer').innerHTML=m+":"+(s<10?'0':'')+s;
time--;
if(time<0) time=600;
},1000);

const nomes=[
"João - SP","Maria - RJ","Carlos - MG","Ana - BA",
"Pedro - CE","Lucas - PE","Fernanda - PR",
"Tiago - Lisboa","Sofia - Porto","Miguel - Braga"
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
</script>

</body>
</html>

