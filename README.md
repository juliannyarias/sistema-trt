# sistema-trt

#Bienvenido 

/*
 <?php

session_start();

if (!isset($_SESSION['usuario'])){
    echo'
         <script>
         alert("Por favor debes iniciar sesión");
         window.location = "index.php";
         </script>
    ';
     session_destroy();
    die();
}
  session_destroy();

?>
<!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8">
	<meta name="viewport" content="width=device.width, inicial-scale=1.0">
	<title>bienvenido a trt</title>
	<link rel="stylesheet" href="assets/css/esti.css">
	 
</head>
<body >
	<header>
	<img src="assets/images/bg2.png" height="120px" width="500px"> 
<nav>
	<a href="bienvenido.php">Inicio</a>
	<a href="program.php">Programas</a>
	<a href="pauta.php">Pautas Comerciales</a>
	<a href="Empleados.php">Empleados</a>
	<a href="formulario.php">Cliente</a>
	<a href="php/cerrar_sesion.php">Cerrar Sesión</a>
</nav>
    </header>
<div class="wrapper">
	<section>
		<h2>Televisora regional del tachira</h2>

		<p>La sede principal de TRT, Televisora Regional del Táchira. Se encuentra ubicado en la carrera 6 entre calles 6 y 7 de la Concordia, San Cristóbal Estado Táchira.</p>

		<img src="assets/images/mapa.png" height="600px" width="800px" >
		<p>
	
		</p>
        <h3>Mision TRT.</h3>
		<p>  La misión de esta prestigiosa televisora es entretener, informar y educar; promover la iniciativa privada; mejorar la calidad de vida y enaltecer el ser y  sentir de nuestra gente.  A través de una programación ajustada a rigurosos estándares de calidad, Televisora Regional del Táchira; además cumple la función de información, orientación, educación y entretenimiento, para contribuir a formar un ciudadano culto, informado, crítico y apto para convivir en una sociedad democrática;  difunde nuestros valores culturales y educativos: las costumbres, el folklore y demás manifestaciones auténticas de nuestro pueblo. También Promociona y divulga las iniciativas orientadas a lograr el desarrollo económico, social y cultural de la región y del país. Reafirma los principios inalienables de la nacionalidad y es portadora de un mensaje de cooperación y hermandad con el vecino país. Por lo tanto Al asumir la función de servicio público que la Constitución Nacional confiere a la radio y la televisión. TRT acata el ordenamiento legal vigente en el país en esta materia y los principios éticos que regulan las telecomunicaciones en el ámbito internacional, desde luego como entidad económica, TRT se propone garantizar a sus accionistas un retorno adecuado de la inversión, sin desmedro de una justa compensación a su personal, una esmerada atención a sus clientes y el cumplimiento de su función de servicio público.</p>
		<h4>vision TRT</h4>
		<p>Su visión  principal son las de crear y mantener una programación y bloques de horario acorde a los gustos del televidente y que generen cifras de audiencia que sean de interés para los anunciantes, gestionar la compra de material audiovisual a los distribuidores nacionales e internacionales; producir programas regionales acordes a la visión y misión del canal; analizar los estudios de audiencia y efectuar los cambios o mejoras que se pudiesen necesitar en la programación; la gerencia de producción está dividida en dos coordinaciones, Producción y Post producción. Para el 2015 TRT, televisora del Táchira, estará posicionada como la voz y la imagen del Táchira y su gente en cualquier parte del mundo.</p>
</section>
</div>
<script src="https://code.jquery.com/jquery-3.5.1.min.js"></script>
<script src="assets/js/script1.js"></script>
</body>
</html>
*/

#Cn

/*
<?php


 $mysqli = new mysqli("localhost","root","","proyectotrt");
/*
if ($conexion) {
	echo  'conectado exitosamente a la base de datos';
}
else{
	echo  'no se ha podido conectar a la base de datos ';
}
*/

?>
*/

#Conex 

/*
<? php
$conn= mysqli_connect('localhost','root','','proyectotrt');

?>
*/

#Conexión

/*
<?php


 $conexion = mysqli_connect("localhost","root","","proyectotrt");
/*
if ($conexion) {
	echo  'conectado exitosamente a la base de datos';
}
else{
	echo  'no se ha podido conectar a la base de datos ';
}
*/

?>
*/

#Em

/*
<?php


 $mysqli = new mysqli("localhost","root","","proyectotrt");
/*
if ($conexion) {
	echo  'conectado exitosamente a la base de datos';
}
else{
	echo  'no se ha podido conectar a la base de datos ';
}
*/

?>
*/

#Emple

/*
<?php
require('fpdf/fpdf.php');
class PDF extends FPDF
{
// Cabecera de página
function Header()
{
     // Arial bold 15
    $this->SetFont('Arial','B',18);
    // Movernos a la derecha
    $this->Cell(60);
    // Título
    $this->Cell(70,10,'Reporte de empleados',1,0,'C');
    // Salto de línea
    $this->Ln(20);

    $this->cell(30,10,'id',1,0,'',0);
    $this->cell(30,10,'nombre',1,0,'',0);
    $this->cell(50,10,'ape_paterno',1,0,'',0);
    $this->cell(50,10,'ape_materno',1,0,'',0);
    $this->cell(30,10,'cargo',1,1,'',0);
    

}

// Pie de página
function Footer()
{
    // Posición: a 1,5 cm del final
    $this->SetY(-15);
    // Arial italic 8
    $this->SetFont('Arial','I',8);
    // Número de página
    $this->Cell(0,10,utf8_decode('página').$this->PageNo().'/{nb}',1,0,'C');
}
}

require 'em.php';
$consulta="SELECT * FROM empleados";
$resultado=$mysqli->query($consulta);

$pdf = new PDF();
$pdf-> AliasNbPages();
$pdf->AddPage();
$pdf->SetFont('Arial','',16);

while ($row= $resultado->fetch_assoc()){

     
	$pdf->cell(30,10,$row['id'],1,0,'',0);
	$pdf->cell(30,10,$row['nombre'],1,0,'',0);
	$pdf->cell(50,10,$row['ape_paterno'],1,0,'',0);
	$pdf->cell(50,10,$row['ape_materno'],1,0,'',0);
	$pdf->cell(30,10,$row['cargo'],1,1,'',0);
}

$pdf->Output();
?>
*/

#Empleados

/*
<html>
<head>
	<meta name="viewport" content="width=device.width, inicial-scale=1.0">
	<title>Programas</title>
	<link rel="stylesheet" href="assets/css/esti.css">
	
</head>
<body>
	<header>
	<img src="assets/images/bg2.png" height="120px" width="500px"> 
<nav>
	<a href="bienvenido.php">Inicio</a>
	<a href="program.php">Programas</a>
	<a href="pauta.php">Pautas Comerciales</a>
	<a href="empleados.php">Empleados</a>
	<a href="formulario.php">clientes</a>
	<a href="php/cerrar_sesion.php">Cerrar Sesión</a>
</nav>
    </header>
<div class="wrapper">
	<section>
		<center><h2>lista de empleados</h2>

	<br>
	<table border="1" >
		<tr>
			<td>id</td>
			<td>nombre</td>
			<td>ape_paterno</td>
		    <td>ape_materno</td>
		    <td>cargo</td>
		</tr>
		<?php
        $sql="SELECT * FROM empleados";
        $result=mysqli_query($conexion,$sql);

        while ($mostrar=mysqli_fetch_array($result)){
		?>

		<tr>
			<td><?php echo $mostrar['id'] ?></td>
			<td><?php echo $mostrar['nombre'] ?></td>
			<td><?php echo $mostrar['ape_paterno'] ?></td>
		    <td><?php echo $mostrar['ape_materno'] ?></td>
		    <td><?php echo $mostrar['cargo'] ?></td>
		</tr>
	<?php 
    }
    ?>
	</table></center>

	<button><a href="emple.php">Haz clic aquí para el PDF</a> </button>
</section>
</div>

<script src="https://code.jquery.com/jquery-3.5.1.min.js"></script>
<script src="assets/js/script1.js"></script>
</body>
</html>
*/

#Formulario

/*
<?php

include 'conexion.php';

$conexion=mysqli_connect('localhost','root','','proyectotrt');

?>

<!DOCTYPE html>
<html>
<head>
	<meta name="viewport" content="width=device.width, inicial-scale=1.0">
	<title>Clientes</title>
	<link rel="stylesheet" href="assets/css/esti.css">
	<link rel="stylesheet" type="text/css" href="css/estilo.a.css">
	<link rel="stylesheet" type="text/css" href="css/estilos_form.css">
	
</head>
<body>
 
	<header>
	<img src="assets/images/bg2.png" height="120px" width="500px"> 
<nav>
	<a href="bienvenido.php">Inicio</a>
	<a href="program.php">Programas</a>
	<a href="pauta.php">Pautas Comerciales</a>
	<a href="empleados.php">empleados</a>
	<a href="formulario.php">clientes</a>
	<a href="php/cerrar_sesion.php">Cerrar Sesión</a>
</nav>
    </header>
<div class="wrapper">
	<section>
		<center><h2>clientes</h2>
    <form method="POST" action="guardar.php" name="form_car" id="form_car" onsubmit="return revisa_form('form_car');">
		<table align="center" border="1" >
			<tr align="center">
			</tr>
			<tr>
				<td align="right">Cedula</td>
				<td><input type="text" id="unicred" name="unicred" size="60" maxlength="10" placeholder="Ingrese el numero de cedula" onkeypress="return SoloNumeros(event)"></td>
			</tr>
			<tr>
				<td align="right">Apellido</td>
				<td><input type="text" id="descripcion" name="descripcion" size="60" maxlength="50" placeholder="Ingrese el apellido" onblur="soloMayusculas('descripcion')"></td>
			</tr>
			<tr>
				<td align="right">Nombre</td>
				<td><input type="text" id="descripcion" name="descripcion" size="60" maxlength="50" placeholder="Ingrese el nombre" onblur="soloMayusculas('descripcion')"></td>
			</tr>
			<tr>
				<td align="right">Fecha de nacimiento</td>
				<td><input type="text" id="descripcion" name="descripcion" size="60" maxlength="10" placeholder="05/01/2002" onblur="soloMayusculas('descripcion')"></td>
			</tr>
			<tr>
                <td align="right">Correo </td>
				<td><input type="text" id="descripcion" name="descripcion" size="60" maxlength="50" placeholder="Ingrese su correo electronico" onblur="soloMayusculas('descripcion')"></td>
			</tr>
			<tr>
				<td align="right">Telefono</td>
				<td><input type="text" id="descripcion" name="descripcion" size="60" maxlength="13" placeholder="0416-0483532" onblur="soloMayusculas('descripcion')"></td>
			</tr>
			<tr>
				<td align="right">Direccion</td>
				<td><input type="text" id="descripcion" name="descripcion" size="60" maxlength="90" placeholder="Ingrese su direccion" onblur="soloMayusculas('descripcion')"></td>
			</tr>
			<tr>
				<td colspan="2" align="center">
					<button><a href="lista.php">guardar</button>
				</td>
			</tr>

	</table></center>

	<button><a href="fpdf.php">Haz clic aquí para el PDF</a> </button>
</section>
</div>

<script src="https://code.jquery.com/jquery-3.5.1.min.js"></script>
<script src="assets/js/script1.js"></script>
<div class="btn-toolbar d-flex justify-content-center mb-3" role="toolbar" aria-label="Toolbar with button groups">
		
	  </div>
</body>
</html>
<script type="text/javascript">
function soloMayusculas(campo_id) 
{
	var cadena = document.getElementById(campo_id).value;
	var cadena2 = cadena.toUpperCase();
	document.getElementById(campo_id).value = cadena2;
}

function SoloNumeros(evt) // solo permite insertar NUMEROS,EL PUNTO, ENTER, ESPACIO, GUION, 
{
	var nav4 = window.Event ? true : false;
	// NOTE: Backspace = 8, Enter = 13, '0' = 48, '9' = 57, '.' = 46
	var key = nav4 ? evt.which : evt.keyCode;
	return (key <= 13 || (key >= 48 && key <= 57));
}

function revisa_form(form_id) 
{
	//Con esta función revisamos los elementos del formulario que se pasa por parámetro
	var formulario = document.getElementById(form_id);	
	var valido = true;
    for (var j=0; j<formulario.elements.length; j++)
    {
        elemento=formulario.elements[j];
        if (elemento.className != 'no_requerido') //Para diferenciar los campos no requeridos en el formulario
        {
	        valor = formulario.elements[j].value;
	        if (valor == null || valor.length == 0)
	        {
	        	alert('[ERROR] El campo '+ formulario.elements[j].name +' no debe estar vací­o');
	        	formulario.elements[j].style.border='1px solid red';
	        	formulario.elements[j].focus();
	        	valido = false;
	        	break;
	        }
    	}
    }
	return valido;
}
</script>
</body>
</html>
*/

#Fpdf

/*
<?php
require('fpdf/fpdf.php');
class PDF extends FPDF
{
// Cabecera de página
function Header()
{
     // Arial bold 15
    $this->SetFont('Arial','B',18);
    // Movernos a la derecha
    $this->Cell(60);
    // Título
    $this->Cell(70,10,'Reporte de Programas',1,0,'C');
    // Salto de línea
    $this->Ln(20);

    $this->cell(30,10,'inicio',1,0,'',0);
    $this->cell(30,10,'final',1,0,'',0);
    $this->cell(30,10,'codigoID',1,0,'',0);
    $this->cell(70,10,'nombre',1,0,'',0);
    $this->cell(30,10,'ubicacion',1,1,'',0);
    

}

// Pie de página
function Footer()
{
    // Posición: a 1,5 cm del final
    $this->SetY(-15);
    // Arial italic 8
    $this->SetFont('Arial','I',8);
    // Número de página
    $this->Cell(0,10,utf8_decode('página').$this->PageNo().'/{nb}',1,0,'C');
}
}

require 'cn.php';
$consulta="SELECT * FROM programas";
$resultado=$mysqli->query($consulta);

$pdf = new PDF();
$pdf-> AliasNbPages();
$pdf->AddPage();
$pdf->SetFont('Arial','',16);

while ($row= $resultado->fetch_assoc()){

     
	$pdf->cell(30,10,$row['inicio'],1,0,'',0);
	$pdf->cell(30,10,$row['final'],1,0,'',0);
	$pdf->cell(30,10,$row['codigoID'],1,0,'',0);
	$pdf->cell(70,10,$row['nombre'],1,0,'',0);
	$pdf->cell(30,10,$row['ubicacion'],1,1,'',0);
}

$pdf->Output();
?>
*/

#Guardar

/*
<?php
//Incluyo el script de utilidades
require_once("utilidades.php");
//Instancio la clase utilidades
$utilities = new utilidades;
//Hago la conexión con la BD
$con = $utilities->conexion();
//Obtengo el valor de la descripción desde el input
$cedula=$_POST["cedula"];
$apellido=$_POST["apellido"];
$nombre=$_POST["nombre"];
$fecha_nac=$_POST["fecha_nac"];
$correo_elec=$_POST["correo_elec"];
$telefono=$_POST["telefono"];
$direccion=$_POST["direccion"];
//Creo la cadena SQL
$sql="insert into estudiante (cedula,apellido,nombre,fecha_nac,correo_elec,telefono,direccion) values ('$cedula','$apellido','$nombre'',$fecha_nac','$correo_elec','$telefono','$direccion')";
//Ejecuto la consulta en la BD
$ok=$con->query($sql);
if ($ok==true)
	echo "Inserción exitosa!";
else
	echo "Falló la inserción";
?>
*/

#Index

/*
<?php

session_start();
if (isset($SESSION['usuario'])) {
	header("location: bienvenido.php");
}
?>


	<!DOCTYPE html>
	<html lang="en">
	<head>
		<meta charset="UTF-8">
		<meta name="viewport" content="width=device-width, initial-scale=1.0">
		<title>	TRT</title>
		<link rel="stylesheet" href="assets/css/estilos.css">
	</head>
	<body>

<main>
		<div class="contenedor__todo">

				<div class="caja__trasera">
					<div class="caja__trasera-login">
						<h3>¿Ya tienes una cuenta?</h3>
						<p>Inicia sesión para entrar en la página </p>
						<button id="btn__iniciar-sesion">Iniciar Sesión </button>
					</div>
					<div class="caja__trasera-register">
						<h3>¿Aún no tienes una cuenta?</h3>
						<p>Regístrate para que puedas iniciar sesión  </p>
						<button id="btn__registrarse">Regístrarse </button>
					</div>
			    </div>	
			<!--formulario de login y registro-->

		    <div class="contenedor__login-register">
		    	<!--login-->

		    	<form action="php/inicio.php" method="POST" class="formulario__login">
		    		<img src="assets/images/bg1.jpg"><h2>Iniciar Sesión</h2>
		    		<input type="text" placeholder="correo electronico" name="correo_electronico">
		    		<input type="password" placeholder="contraseña" name="contra">
		    		<button>Entrar</button>
		    	</form>
		    	<!--registro-->
                 <form action="php/registro.php" method="POST" class="formulario__register">
                   <img src="assets/images/bg1.jpg"><h2>Registrarse</h2>
                    <input type="text" placeholder="Nombre completo" name="nombre_completo">
                    <input type="text" placeholder="Correo electronico"name="correo_electronico">
                    <input type="text" placeholder="Usuario"name="usuario">
                    <input type="password" placeholder="contraseña" name="contra">
                    <button>Registrarse</button>
                 </form>
		    </div>
		</div>
</main>

<script src="assets/js/script.js"></script>
	
	</body>
	</html>
*/

#Lista

/*
<?php
//Incluyo el script de utilidades
require_once("utilidades.php");
//Instancio la clase utilidades
$utilities = new utilidades;
//Hago la conexión con la BD
$con = $utilities->conexion();
//Creo la cadena SQL
$sql="SELECT * FROM cliente";
//Ejecuto la consulta en la BD
$ok=$con->query($sql); //En este caso el query devuelve un juego de registros en un objeto
if ($ok==true)
{
 ?>
 <html>
 <head>
  <meta charset="utf-8">
  
  <link rel="stylesheet" type="text/css" href="assets/css/estilo.a.css">
		<link rel="stylesheet" type="text/css" href="assets/css/estilos_form.css">
  <link rel="stylesheet" href="assets/css/esti.css">
  <title>Listar cliente</title>
 </head>
 <header>
  <img src="assets/images/bg2.png" height="120px" width="500px"> 
<nav>
  <a href="bienvenido.php">Inicio</a>
  <a href="program.php">Programas</a>
  <a href="pauta.php">Pautas Comerciales</a>
  <a href="empleados.php">empleados</a>
  <a href="formulario.php">clientes</a>
  <a href="php/cerrar_sesion.php">Cerrar Sesión</a>
</nav>
    </header>
<div class="wrapper">
  <section>
 <body > 
   <table align="center" class="tabla_grande">
          <tr align="center">
              <td colspan="7" id="encabezado" class="cabecera_tabla">Listar clientes</td>
				  </tr>
    <tr>
     <td align="center" class="cabecera_columna">Cedula</td>
     <td align="center" class="cabecera_columna">Apellido</td>
     <td align="center" class="cabecera_columna">Nombre</td>
     <td align="center" class="cabecera_columna">Fecha-nac</td>
     <td align="center" class="cabecera_columna">correo</td>
     <td align="center" class="cabecera_columna">telefono</td>
     <td align="center" class="cabecera_columna">direccion</td>
    </tr>
    <?php
     while (($fila=$ok->fetch_assoc())>0) //Recorre fila por fila el juego de registros y asigna un vector llamado fila con los datos de cada registo
     {
      echo "<tr>";
      echo "<td align='center'>".$fila['cedula']."</td>";
      echo "<td align='center'>".$fila['apellido']."</td>";
      echo "<td align='center'>".$fila['nombre']."</td>";
      echo "<td align='center'>".$fila['fecha_nac']."</td>";
      echo "<td align='center'>".$fila['correo']."</td>";
      echo "<td align='center'>".$fila['telefono']."</td>";
      echo "<td align='center'>".$fila['direccion']."</td>";
      echo "</tr>";
     }
    ?>
   </table>
   <script src="https://code.jquery.com/jquery-3.5.1.min.js"></script>
<script src="assets/js/script1.js"></script>
 </body>
 </form>
 <div class="btn-toolbar d-flex justify-content-center mb-3" role="toolbar" aria-label="Toolbar with button groups">
		<div class="btn-group mr-2" role="group" aria-label="First group" >
			<center></center>
		</div>
	  </div>
 </html>
<?php
}
else
{
 echo "Falló la consulta";
}
*/

#Pauta

/*
<?php

include 'conexion.php';

$conexion=mysqli_connect('localhost','root','','proyectotrt');

?>

<!DOCTYPE html>
<html>
<head>
	<meta name="viewport" content="width=device.width, inicial-scale=1.0">
	<title>Pautas comerciales</title>
	<link rel="stylesheet" href="assets/css/esti.css">
	
</head>
<body>
	<header>
	<img src="assets/images/bg2.png" height="120px" width="500px"> 
<nav>
	<a href="bienvenido.php">Inicio</a>
	<a href="program.php">Programas</a>
	<a href="pauta.php">Pautas Comerciales</a>
	<a href="empleados.php">empleados</a>
	<a href="formulario.php">Cliente</a>
	<a href="php/cerrar_sesion.php">Cerrar Sesión</a>
</nav>
    </header>
<div class="wrapper">
	<section>
		<center><h2>lista de pautas comerciales</h2>

	<br>
	<center><table border="1" >
		<tr>
			<td>cuna</td>
			<td>Nombre</td>
			<td>segundo</td>
		    
		</tr>
		<?php
        $sql="SELECT * FROM pautas";
        $result=mysqli_query($conexion,$sql);

        while ($mostrar=mysqli_fetch_array($result)){
		?>

		<tr>
			<td><?php echo $mostrar['cuna'] ?></td>
			<td><?php echo $mostrar['Nombre'] ?></td>
			<td><?php echo $mostrar['segundo'] ?></td>
		   
		</tr>
	<?php 
    }
    ?>
	</table></center>
	
	<button><a href="pdf.php">Haz clic aquí para el PDF</a> </button>
	
</section>
</div>

<script src="https://code.jquery.com/jquery-3.5.1.min.js"></script>
<script src="assets/js/script1.js"></script>
</body>
</html>
*/

#Pd

/*
<?php


 $mysqli = new mysqli("localhost","root","","proyectotrt");
/*
if ($conexion) {
	echo  'conectado exitosamente a la base de datos';
}
else{
	echo  'no se ha podido conectar a la base de datos ';
}
*/

?>
*/

#Pdf

/*
<?php
require('fpdf/fpdf.php');
class PDF extends FPDF
{
// Cabecera de página
function Header()
{
     // Arial bold 15
    $this->SetFont('Arial','B',18);
    // Movernos a la derecha
    $this->Cell(60);
    // Título
    $this->Cell(70,10,'Reporte de Pautas',1,0,'C');
    // Salto de línea
    $this->Ln(20);

    $this->cell(50,10,'cuna',1,0,'',0);
    $this->cell(80,10,'Nombre',1,0,'',0);
    $this->cell(50,10,'segundo',1,1,'',0);
    

}

// Pie de página
function Footer()
{
    // Posición: a 1,5 cm del final
    $this->SetY(-15);
    // Arial italic 8
    $this->SetFont('Arial','I',8);
    // Número de página
    $this->Cell(0,10,utf8_decode('página').$this->PageNo().'/{nb}',1,0,'C');
}
}

require 'pd.php';
$consulta="SELECT * FROM pautas";
$resultado=$mysqli->query($consulta);

$pdf = new PDF();
$pdf-> AliasNbPages();
$pdf->AddPage();
$pdf->SetFont('Arial','',16);

while ($row= $resultado->fetch_assoc()){

     
	$pdf->cell(50,10,$row['cuna'],1,0,'',0);
	$pdf->cell(80,10,$row['Nombre'],1,0,'',0);
	$pdf->cell(50,10,$row['segundo'],1,1,'',0);
}

$pdf->Output();
?>
*/

#Program

/*
<?php

include 'conexion.php';

$conexion=mysqli_connect('localhost','root','','proyectotrt');

?>

<!DOCTYPE html>
<html>
<head>
	<meta name="viewport" content="width=device.width, inicial-scale=1.0">
	<title>Programas</title>
	<link rel="stylesheet" href="assets/css/esti.css">
	
</head>
<body>
	<header>
	<img src="assets/images/bg2.png" height="120px" width="500px"> 
<nav>
	<a href="bienvenido.php">Inicio</a>
	<a href="program.php">Programas</a>
	<a href="pauta.php">Pautas Comerciales</a>
	<a href="empleados.php">empleados</a>
	<a href="formulario.php">Cliente</a>
	<a href="php/cerrar_sesion.php">Cerrar Sesión</a>
</nav>
    </header>
<div class="wrapper">
	<section>
		<center><h2>lista de programas televisivos</h2>

	<br>
	<table border="1" >
		<tr>
			<td>inicio</td>
			<td>final</td>
			<td>codigoID</td>
		    <td>nombre</td>
		    <td>ubicacion</td>
		</tr>
		<?php
        $sql="SELECT * FROM programas";
        $result=mysqli_query($conexion,$sql);

        while ($mostrar=mysqli_fetch_array($result)){
		?>

		<tr>
			<td><?php echo $mostrar['inicio'] ?></td>
			<td><?php echo $mostrar['final'] ?></td>
			<td><?php echo $mostrar['codigoID'] ?></td>
		    <td><?php echo $mostrar['nombre'] ?></td>
		    <td><?php echo $mostrar['ubicacion'] ?></td>
		</tr>
	<?php 
    }
    ?>
	</table></center>

	<button><a href="fpdf.php">Haz clic aquí para el PDF</a> </button>
</section>
</div>

<script src="https://code.jquery.com/jquery-3.5.1.min.js"></script>
<script src="assets/js/script1.js"></script>
</body>
</html>
*/

#Utilidades

/*
<?php
class utilidades
{
	function conexion()
	{
		$con = new mysqli('localhost','root','','proyectotrt');
		if ($con->connect_errno)
		{
		    echo "Fallo al conectar al servidor: (" . $con->connect_errno . ") " . $con->connect_error;
		}		
		else		
			return $con;
	}
}
?>
*/




