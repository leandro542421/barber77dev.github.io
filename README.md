<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Jonocampo77 Barbería</title>

<style>
.galeria{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:20px;
}

.foto{
    width:100%;
    height:300px;
    object-fit:cover;
    border:2px solid #d4af37;
    border-radius:10px;
}
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial, sans-serif;
}

body{
    background:#0d0d0d;
    color:white;
}

header{
    text-align:center;
    padding:40px 20px;
}

.logo{
    width:220px;
    height:220px;
    border-radius:50%;
    border:4px solid #d4af37;
    object-fit:cover;
    box-shadow:0 0 25px rgba(212,175,55,.5);
}

h1{
    margin-top:20px;
    color:#d4af37;
    font-size:3rem;
}

.subtitulo{
    color:#bdbdbd;
    margin-top:10px;
}

.menu{
    display:flex;
    justify-content:center;
    flex-wrap:wrap;
    gap:15px;
    margin:40px 0;
}

.menu button{
    background:#d4af37;
    color:black;
    border:none;
    padding:12px 25px;
    border-radius:30px;
    font-size:16px;
    font-weight:bold;
    cursor:pointer;
    transition:.3s;
}

.menu button:hover{
    transform:scale(1.05);
}

.contenido{
    display:none;
    max-width:900px;
    margin:auto;
    padding:30px;
    text-align:center;
}

.activo{
    display:block;
}

h2{
    color:#d4af37;
    margin-bottom:20px;
}

.btn{
    display:inline-block;
    background:#d4af37;
    color:black;
    text-decoration:none;
    padding:12px 25px;
    border-radius:30px;
    font-weight:bold;
    margin-top:15px;
}

.galeria{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:20px;
}

.foto{
    background:#1a1a1a;
    border:2px solid #d4af37;
    border-radius:12px;
    height:250px;
    display:flex;
    justify-content:center;
    align-items:center;
    color:#d4af37;
    font-size:20px;
}

footer{
    margin-top:50px;
    text-align:center;
    padding:20px;
    border-top:1px solid #333;
    color:#888;
}

</style>
</head>

<body>

<header>

    <!-- Cambia logo.png por el nombre de tu logo -->
    <img src="barber.jpeg" alt="Logo Barbería" class="logo">

    <h1>JONOCAMPO77</h1>

    <p class="subtitulo">
        Barbería Profesional
    </p>

</header>

<div class="menu">

    <button onclick="mostrar('inicio')">
        Inicio
    </button>

    <button onclick="mostrar('sobre')">
        Sobre mí
    </button>

    <button onclick="mostrar('galeria')">
        Galería
    </button>

    <button onclick="mostrar('contacto')">
        Contacto
    </button>

</div>

<div id="inicio" class="contenido activo">

    <h2>Bienvenido</h2>

    <p>
        Bienvenido a Jonocampo77 Barbería.
        Estilo, experiencia y calidad en cada corte.
    </p>

    <a
        href="https://www.instagram.com/jonocampo77?igsh=aHo0bGN3aGdsOW1y"
        target="_blank"
        class="btn">

        Ver Instagram

    </a>

</div>

<div id="sobre" class="contenido">

    <h2>Sobre mí</h2>

    <p>
        Soy barbero profesional con más de 15 años de experiencia.
        Especialista en cortes modernos, clásicos y arreglo de barba.

        No vendemos un corte, vendemos una experiencia.
    </p>

</div>

<div id="galeria" class="contenido">

    <h2>Galería</h2>

    <div class="galeria">

    <div class="galeria">
    <img src="ubicacion.jpeg" class="foto">   

    <img src="corteprimero.jpg" class="foto">

    <img src="corte2.jpg" class="foto">

    <img src="corte3.jpg" class="foto">

    <img src="corte6.jpeg" class="foto">

    <img src="corte7.jpeg" class="foto">

</div>


    </div>

    <br>

    <p>
    
    </p>

</div>

<div id="contacto" class="contenido">

    <h2>Contacto</h2>

    <p>
        Agenda tu cita por WhatsApp.
    </p>

    <a
        href="https://wa.me/573207440896"
        target="_blank"
        class="btn">

        +57 320 744 0896

    </a>

</div>

<footer>

    © 2026 Jonocampo77 Barbería

</footer>

<script>

function mostrar(id){

    let secciones =
    document.querySelectorAll(".contenido");

    secciones.forEach(function(sec){
        sec.classList.remove("activo");
    });

    document
    .getElementById(id)
    .classList.add("activo");
}

</script>

</body>
</html>
