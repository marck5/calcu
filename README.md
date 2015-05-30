# calcu
calculadora
<!DOCTYPE HTML-->
<html>
<head>
<meta charset="UTF-8">
<link rel="stylesheet" href="css/jquery-ui.css">
<link rel="stylesheet" href="css/jquery.mobile-1.4.5.min.css">
<script type="text/javascript" src="js/jquery-ui.js"> </script>
<script type="text/javascript" src="js/jquery.min.js"> </script>
<script type="text/javascript" src="js/jquery.mobile-1.4.5.min.js"> </script> 
<script>
    $(document).ready(function (){
        $("#btnSuma").click(function (){
            var n1=parseInt($("#num1").val());
            var n2=parseInt($("#num2").val());
            var resultado=$("#resultado");
            resultado.val(n1+n2);
        })
        
        $("#btnResta").click(function (){
            var n1=parseInt($("#num1").val());
            var n2=parseInt($("#num2").val());
            var resultado=$("#resultado");
            resultado.val(n1-n2);
        })
        
        $("#btnDiv").click(function (){
            var n1=parseInt($("#num1").val());
            var n2=parseInt($("#num2").val());
            var resultado=$("#resultado");
            resultado.val(n1/n2);
        })
        
        $("#btnMulti").click(function (){
            var n1=parseInt($("#num1").val());
            var n2=parseInt($("#num2").val());
            var res=$("#resultado");
            res.val(n1*n2);
        })
    })
</script>
<style type="text/css"> 
    p{text-align: center;}
</style>
</head>
<body>
<div data-role="page" id="Principal">
        <div data-role="header">
            <p> Mi primera aplicación móvil</p> 
        </div> 
        <div data-role="content">
            <a href="#Articulo" data-role="button" data-transition="slideup">Abrir Página con slideup</a>
            <a href="#Articulo" data-role="button" data-transition="slidedown">Abrir Página con slidedown</a>
            <a href="#Articulo" data-role="button" data-transition="flip">Abrir Página con flip</a>
            <a href="#Articulo" data-role="button" data-transition="pop">Abrir Página con pop</a>
        </div>
        <div data-role="footer">
            <p>pie de la aplicación móvil</p>
        </div>
</div>
    
<div data-role="page" id="Articulo">
        <div data-role="header">
            <a href="#Principal" data-role="burron" data-transition="flip">Regresar</a> <p>Articulo</p> 
        </div> 
        <div data-role="content">
            <p>Contenido del Articulo</p>
            <img src="images/descarga.jpg">
            <label for="num1">Número 1:</label>
            <input type="text" id="num1" placeholder="Número 1">
            <label for="num1">Número 2:</label>
            <input type="text" id="num2" placeholder="Número 2">
            <input type="text" id="resultado" placeholder="Resultado">
            <input type="button" value="Sumar" id="btnSuma">
            <input type="button" value="Restar" id="btnResta">
            <input type="button" value="Dividir" id="btnDiv">
            <input type="button" value="Multiplicar" id="btnMulti">
        </div>
        <div data-role="footer">
            <p>Pie del Articulo</p>
        </div>
</div>
</body>
</html>11
