<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Entendiendo el sexting – Modelo 3D</title>
<style>
:root{--bg1:#1b2a3d;--bg2:#070d15;--paper:#dcebf7;--paper2:#c4dcf0;--head:#8fbfe4;--ink:#0f2a4a;--navy:#1d3f6e;--blue:#3b82c4}
*{box-sizing:border-box;margin:0}
html,body{height:100%;overflow:hidden;color-scheme:dark}
body{background:radial-gradient(ellipse at 50% 30%,var(--bg1),var(--bg2));font-family:"Trebuchet MS","Segoe UI",Arial,sans-serif;user-select:none;touch-action:none;cursor:grab}
body:active{cursor:grabbing}
#view{position:absolute;inset:0;display:flex;align-items:center;justify-content:center;perspective:1600px}
#scale{width:840px;height:680px;transform-style:preserve-3d}
#rig{position:relative;width:840px;height:680px;transform-style:preserve-3d}
.floor{position:absolute;left:60px;top:640px;width:720px;height:90px;background:radial-gradient(ellipse,rgba(0,0,0,.55),transparent 70%);transform:rotateX(90deg)}
.panel{position:absolute;top:110px;height:540px;background:linear-gradient(180deg,var(--paper),var(--paper2));color:var(--ink);padding:14px 12px;overflow:hidden;backface-visibility:visible;box-shadow:inset 0 0 0 3px #fff6}
.center{left:210px;width:420px}
.left{left:0;width:210px;transform-origin:100% 50%;transform:rotateY(var(--w))}
.right{left:630px;width:210px;transform-origin:0 50%;transform:rotateY(calc(var(--w) * -1))}
.banner{position:absolute;left:150px;top:0;width:540px;height:100px;background:var(--head);display:flex;align-items:center;justify-content:center;text-align:center;font-weight:900;font-size:25px;line-height:1.15;color:var(--ink);transform:translateZ(-4px);box-shadow:0 0 0 3px #fff6}
.tag{background:var(--head);font-weight:800;font-size:13px;padding:7px 8px;border-radius:4px;margin-bottom:10px;text-align:center}
h3{font-size:19px;font-weight:900;line-height:1.1;text-align:center;margin:6px 0 8px}
h4{font-size:15px;font-weight:900;line-height:1.1;text-align:center;margin:8px 0 6px}
ul{list-style:none;font-size:12.5px;font-weight:600;line-height:1.5;padding-left:4px}
li:before{content:"• ";color:var(--blue)}
.cols{display:grid;grid-template-columns:1fr 1fr;gap:10px}
.box{background:#fff9;border-radius:6px;padding:7px;font-size:11px}
.box b{display:block;background:var(--navy);color:#fff;text-align:center;padding:3px;margin-bottom:4px;font-size:10.5px}
.foot{position:absolute;left:0;right:0;bottom:0;background:var(--navy);color:#fff;font-size:10px;font-weight:700;padding:8px 10px;text-align:center}
.concl{background:var(--head);border-radius:6px;padding:8px;margin-top:6px;font-size:11px;font-weight:600;line-height:1.35}
.concl b{display:block;font-size:14px;margin-bottom:3px}
.ph{height:78px;border-radius:6px;background:linear-gradient(135deg,#9db9d3,#5f84a8);display:flex;align-items:center;justify-content:center;font-size:12px;font-weight:700;color:#fff;margin:6px 0;text-align:center;padding:6px}
#ui{position:fixed;left:0;right:0;bottom:max(12px,env(safe-area-inset-bottom));display:flex;gap:8px;justify-content:center;flex-wrap:wrap;padding:0 10px;z-index:5}
button{font:inherit;font-weight:700;font-size:13px;color:#fff;background:#ffffff1f;border:1px solid #ffffff40;border-radius:20px;padding:9px 14px;cursor:pointer}
button:hover,button.on{background:#3b82c4}
#hint{position:fixed;top:max(10px,env(safe-area-inset-top));left:0;right:0;text-align:center;color:#ffffffa0;font-size:12px;pointer-events:none}
</style>
</head>
<body>
<div id="hint">Arrastrá para girar · rueda o +/− para zoom</div>
<div id="view"><div id="scale"><div id="rig">
  <div class="floor"></div>
  <div class="banner">ENTENDIENDO EL SEXTING:<br>LOS TRES PILARES DEL ABUSO</div>

  <section class="panel left">
    <div class="tag">EL AGRESOR</div>
    <h3>ESTRATEGIA DE MANIPULACIÓN</h3>
    <div class="ph">Mensajes que parecen amables</div>
    <ul><li>Falsa amistad y confianza</li><li>Validación emocional</li><li>Aislamiento gradual</li><li>Normalización del secreto</li></ul>
    <div class="ph">Contacto por celular, a escondidas</div>
  </section>

  <section class="panel center">
    <div class="cols">
      <div><div class="tag">EL MENOR</div><h4>FACTORES DE VULNERABILIDAD</h4>
        <ul><li>Baja autoestima</li><li>Necesidad de afecto</li><li>Búsqueda de validación</li><li>Sensación de soledad</li></ul></div>
      <div><div class="tag">EL ENTORNO DIGITAL</div><h4>FACILITADORES Y MEDIACIÓN</h4>
        <ul><li>Redes sociales y apps</li><li>Falsa identidad (perfiles fakes)</li><li>Falta de supervisión adulta</li><li>Brecha digital</li></ul></div>
    </div>
    <h4 style="font-size:17px;margin-top:12px">EL VÍNCULO LETAL:<br>DONDE CONVERGEN LOS FACTORES</h4>
    <svg viewBox="0 0 300 190" width="100%" height="190" aria-label="Diagrama de Venn: agresor, menor, entorno">
      <g fill-opacity=".55"><circle cx="150" cy="62" r="55" fill="#1d6fb8"/><circle cx="110" cy="122" r="55" fill="#4f9ad6"/><circle cx="190" cy="122" r="55" fill="#fff"/></g>
      <g font-weight="800" font-size="13" text-anchor="middle" fill="#0f2a4a"><text x="150" y="48" fill="#fff">AGRESOR</text><text x="85" y="140">MENOR</text><text x="215" y="140">ENTORNO</text><text x="150" y="104" font-size="12">GROOMING</text></g>
    </svg>
    <div class="cols" style="margin-top:4px">
      <div class="box"><b>SEÑALES DE ALERTA</b>Secretismo · cambios en la conversación · nuevos "amigos" online</div>
      <div class="box"><b>MEDIDAS DE PREVENCIÓN</b>Diálogo abierto · control parental · educación digital</div>
    </div>
    <div class="foot">AYUDA Y APOYO: Línea 102 (niñez y adolescencia) · Línea 137 · denunciá el perfil en la plataforma</div>
  </section>

  <section class="panel right">
    <div class="tag">PREVENCIÓN Y ACCIÓN</div>
    <div class="ph" style="height:70px">Adulto y menor dialogando</div>
    <h3>CÓMO ACTUAR: CONSEJOS CLAVE</h3>
    <ul><li>Fomentar la confianza en casa</li><li>Educación digital temprana</li><li>Reportar en plataformas</li><li>Buscar ayuda profesional</li></ul>
    <div class="concl"><b>CONCLUSIÓN FINAL</b>El grooming no es culpa de la víctima. Comprender estos tres factores es el primer paso para prevenir y proteger a nuestros menores en el entorno digital.</div>
  </section>
</div></div></div>

<div id="ui">
  <button data-v="0,0">Frente</button>
  <button data-v="-45,0">Izquierda</button>
  <button data-v="45,0">Derecha</button>
  <button data-v="0,-62">Desde arriba</button>
  <button id="auto">Giro auto</button>
  <button id="zi">+</button><button id="zo">−</button>
  <button id="fs">Pantalla completa</button>
</div>

<script>
var ry=-18, rx=-6, zoom=1, tY=ry, tX=rx, auto=false, t0=0, drag=false, lx=0, ly=0;
var rig=document.getElementById('rig'), sc=document.getElementById('scale');
function fit(){var s=Math.min(innerWidth/900, (innerHeight-90)/700);sc.style.transform='scale('+(s*zoom)+')';}
function draw(){rig.style.transform='rotateX('+(-rx)+'deg) rotateY('+ry+'deg)';}
function loop(t){
  if(auto){ry=Math.sin(t/2200)*55;tY=ry;rx=-6;tX=rx;}
  else if(!drag){ry+=(tY-ry)*.12;rx+=(tX-rx)*.12;}
  draw();requestAnimationFrame(loop);
}
document.documentElement.style.setProperty('--w','28deg');
addEventListener('pointerdown',function(e){if(e.target.closest('#ui'))return;drag=true;auto=false;lx=e.clientX;ly=e.clientY;});
addEventListener('pointermove',function(e){if(!drag)return;ry=Math.max(-85,Math.min(85,ry+(e.clientX-lx)*.4));rx=Math.max(-70,Math.min(25,rx-(e.clientY-ly)*.3));tY=ry;tX=rx;lx=e.clientX;ly=e.clientY;});
addEventListener('pointerup',function(){drag=false;});
addEventListener('wheel',function(e){zoom=Math.max(.5,Math.min(2.2,zoom-e.deltaY*.001));fit();},{passive:true});
addEventListener('resize',fit);
document.querySelectorAll('[data-v]').forEach(function(b){b.onclick=function(){var v=b.dataset.v.split(',');tY=+v[0];tX=+v[1];auto=false;};});
document.getElementById('auto').onclick=function(){auto=!auto;this.classList.toggle('on',auto);};
document.getElementById('zi').onclick=function(){zoom=Math.min(2.2,zoom+.15);fit();};
document.getElementById('zo').onclick=function(){zoom=Math.max(.5,zoom-.15);fit();};
document.getElementById('fs').onclick=function(){try{(document.fullscreenElement?document.exitFullscreen():document.documentElement.requestFullscreen());}catch(e){}};
fit();requestAnimationFrame(loop);
</script>
</body>
</html>
