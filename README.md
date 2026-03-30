<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<title>Merca Wheels CT</title>

<style>
body{
    margin:0;
    font-family:'Segoe UI', sans-serif;
    background:linear-gradient(135deg, #000000, #1a1a1a);
    color:white;
}

/* CONTENEDOR */
.container{
    padding:20px;
}

/* HEADER */
header{
    text-align:center;
    font-size:50px;
    font-weight:bold;
    color:#ff6600;
    letter-spacing:2px;
    margin-bottom:20px;
    animation:fadeIn 1s ease;
}

/* BOTONES NAV */
.nav{
    text-align:center;
    margin-bottom:25px;
}

.nav button{
    background:linear-gradient(45deg, orange, red);
    border:none;
    padding:12px 25px;
    margin:10px;
    border-radius:30px;
    color:white;
    font-weight:bold;
    cursor:pointer;
    transition:0.3s;
}

.nav button:hover{
    transform:scale(1.1);
}

/* SECCIONES */
.seccion{ display:none; }
.activa{ display:block; }

/* GRID */
.productos{
    display:grid;
    grid-template-columns:repeat(auto-fit, minmax(230px, 1fr));
    gap:20px;
}

/* TARJETAS */
.card{
    background:linear-gradient(145deg, #111, #1f1f1f);
    border-radius:15px;
    padding:20px;
    text-align:center;
    box-shadow:0 0 15px rgba(255,100,0,0.2);
    transition:0.4s;
    animation:fadeUp 0.6s ease;
}

.card:hover{
    transform:translateY(-10px) scale(1.05);
    box-shadow:0 0 25px rgba(255,100,0,0.6);
}

.card h3{
    font-size:16px;
    margin-bottom:10px;
}

.precio{
    color:gold;
    font-size:20px;
    font-weight:bold;
}

/* CONTACTO */
.contacto{
    margin-top:40px;
    background:#000;
    padding:20px;
    border-radius:15px;
    text-align:center;
    animation:fadeIn 1s ease;
}

/* ANIMACIONES */
@keyframes fadeIn{
    from{opacity:0;}
    to{opacity:1;}
}

@keyframes fadeUp{
    from{
        opacity:0;
        transform:translateY(20px);
    }
    to{
        opacity:1;
        transform:translateY(0);
    }
}
</style>

<script>
function mostrar(seccion){
    document.getElementById("basicos").classList.remove("activa");
    document.getElementById("packs").classList.remove("activa");
    document.getElementById(seccion).classList.add("activa");
}
</script>

</head>
<body>

<div class="container">

<header>MERCA WHEELS CT</header>

<div class="nav">
    <button onclick="mostrar('basicos')">🔥 BÁSICOS</button>
    <button onclick="mostrar('packs')">📦 5 PACKS</button>
</div>

<!-- BASICOS -->
<div id="basicos" class="seccion activa">
<div class="productos">

<div class="card"><h3>DATSUN 240Z</h3><div class="precio">$3.25</div></div>
<div class="card"><h3>FORD MUSTANG GTD</h3><div class="precio">$3.25</div></div>
<div class="card"><h3>BUGATTI BOLIDE</h3><div class="precio">$3.25</div></div>
<div class="card"><h3>LAMBORGHINI SESTO ELEMENTO</h3><div class="precio">$3.25</div></div>
<div class="card"><h3>67 SHELBY GT500</h3><div class="precio">$3.25</div></div>
<div class="card"><h3>CUSTOM 18 FORD MUSTANG GT</h3><div class="precio">$3.25</div></div>
<div class="card"><h3>PORSCHE 911 GT3</h3><div class="precio">$3.25</div></div>
<div class="card"><h3>NISSAN SKYLINE GT-R (BCNR33)</h3><div class="precio">$3.25</div></div>
<div class="card"><h3>BACK TO THE FUTURE TIME MACHINE - HOVER MODE</h3><div class="precio">$7.25</div></div>
<div class="card"><h3>PASS N GO</h3><div class="precio">$3.50</div></div>
<div class="card"><h3>BATMAN ARKHAM KNIGHT BATMOBILE (AZUL)</h3><div class="precio">$5.00</div></div>

</div>
</div>

<!-- PACKS -->
<div id="packs" class="seccion">
<div class="productos">

<div class="card"><h3>HW REMOTE ADVENTURES</h3><div class="precio">$13</div></div>
<div class="card"><h3>HW FLAMES</h3><div class="precio">$13</div></div>
<div class="card"><h3>MOPAR</h3><div class="precio">$13</div></div>

</div>
</div>

<div class="contacto">
<h2>CONTACTO</h2>
<p>📱 WhatsApp: 70260978</p>
<p>📧 mercawheels0ct0@gmail.com</p>
<p>📸 Instagram: merca__wheels__ct</p>
</div>

</div>

</body>
</html>
