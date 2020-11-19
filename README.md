
<html>
<head>
<title>Productos químicos de limpieza</title> 
</head>
<body>
	<style type="text/css">
* { margin: auto; padding: 0; text-align: center }
#cabecera { font: bold 1.3em verdana; background-color: #feffe4;  }
h1 { text-align: center ; padding: 0.5em }
#menu { float: left; width: 25%; background-color: #e3f2ff; }
#menu img { width: 35%; margin: 5%; cursor: pointer; }
#principal { float: left; width: 75%; }
#visor { width: 60%; margin: 10% }
#visor img { width: 100% }
</style>
<script type="text/javascript">
window.onload = function() { //tras cargar la página ...
visor1=document.getElementById("visor"); //referencia al visor
mititulo=document.getElementById("titulo"); //referencia al pie de foto
}
function mifoto(num) { //cambiar la imagen
         f="foto"+num+".jpg"; //ruta de la nueva imagen
         document.images["fotoVisor"].src=f; //cambiar imagen
         t=document.images["fotos"+num].alt; //texto de pie de foto
         mititulo.innerHTML=t; //cambiar pie de foto
         }
</script>
<div id="cabecera">
<h1>Productos químicos de limpieza</h1>
</div>
<div id="menu">
<img src='foto1.jpg' alt='1. Amoniaco.' name='fotos1' onclick="mifoto(1)"/>
<img src='foto2.jpg' alt='2. Blanqueador Clorox.' name='fotos2' onclick="mifoto(2)"/>
<img src='foto3.jpg' alt='3. Limpiador antibacterial.' name='fotos3' onclick="mifoto(3)"/>
<img src='foto4.jpg' alt='4. Limpiador para pisos.' name='fotos4' onclick="mifoto(4)"/>
<img src='foto5.jpg' alt='5. Desinfectante lavanda fabuloso.' name='fotos5' onclick="mifoto(5)"/>
<img src='foto6.jpg' alt='6. Desinfectante en aerosol cítrico.' name='fotos6' onclick="mifoto(6)"/>
<img src='foto7.jpg' alt='7. Desinfectante Sanisol.' name='fotos7' onclick="mifoto(7)"/>
<img src='foto8.jpg' alt='8. Limpiador para acero inoxidable.' name='fotos8' onclick="mifoto(8)"/>
</div>
<div id="principal">
<div id="visor">
   <img src='foto1.jpg' alt='1. Amoniaco.' name='fotoVisor'/>
   <div id="titulo">1. Amoniaco.</div>
   </div>
</div>
</body>
</html> 
