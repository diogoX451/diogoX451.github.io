# diogoX451.github.io
 git remote add origin https://github.com/diogoX451/diogoX451.github.io.git
 git push -u origin master

<meta charset="utf-8">



 <title>TRANSFORMAÇÃO DE TEMPERATURA</title>
 <canvas width="600" height="400" 
 style="border: 1px solid black;">
 	

 </canvas>
 <br>
 <br>
   Se gostar do programa, me segue lá no insta e da um apoio!
    <br>
      Você tiver uma ideia que possa me ajudar a melhorar o programa, pode mandar um direct.
       <br>
         Se ocorrer algum bug me mande um direct também!
       <p><a href="https://www.instagram.com/xs.dioguinho/?hl=es"> clique aqui</a></p>
  <br>
   

 <h3>Instruções</h3>


   <br>
     POR FAVOR REINICA A PÁGINA PARA CALCULAR OUTROS NUMEROS!!
     <br>
      <br>
      <h5> * Numero 1 calcula de C° para F°</h5>
        <br>
         <br>
         <h5>*Nuemero 2 calcula de F° para K</h5>
          <br>
           <br>
          <h5>* Nuemro 3 calcula K para C°</h5>
             <br>
              <br>
          <h5> * Numero 4 calcula F° para C°</h5>
                <br>
                 <br>
            <h5>* Numero 5 calcula K para F° </h5>       


<script>
	 alert("Seja Bem-vindo, esse programa e simples, com tempo vai ter melhorias. A ordem para calcular as transformações de temperaturas são! 1 de C° para F°, 2 F° para K, 3 K para C°, 4 F° para C°, 5 K para F° ");
	// Parte do canvas 
	var canvas = document.querySelector('canvas');
	 var brush = canvas.getContext('2d')
    
    //TITULO
     brush.font ='29px arial';
     brush.fillStyle="black"
     brush.fillText("BEM-VINDO :)", 200, 40);

    //INFORMAÇÕES

    brush.font = '15px time news roman';
    brush.fillStyle = "green";
    brush.fillText("Esse software e uma base, para ajudar você!!", 10, 100);

    brush.font = '15px time news roman';
    brush.fillStyle = "graw";
    brush.fillText("Direitos: @xs.dioguinho", 400, 390);


    

	// FIM DO CANVAS E INICIO DO PROGRAMA   
	var c = prompt("Qual unidade você deseja calcular?");
     //1 para calcular C° para F°
     // 2 para calacular F° para K
     // 3 para calcular K para C°
     


	function salt(){

		document.write('<br><br>');

	}

	function frase (x){

		document.write(x);
		 salt();
	}

    function celcius(){

       var C = parseInt(prompt(" Qual valor em Celcius?"));
		var calculo = ((C * 9) /5) + 32;
		  brush.font = "15px time news roman";
		   brush.fillStyle = "red"
		    brush.fillText ("Transformação de C° para F° é " + calculo, 20, 150);

    }
 
     

     if(c == 1){

     	celcius();

     }

    function Fahrenheit() {
      

    	var f  = parseInt(prompt('Qual valor em Fahrenheit?'));
         var calculo = ((f - 32) * 5)/9 + 273;
          brush.font ="15x time news roman"
           brush.fillStyle = "blue";
            brush.fillText(" Transformação de F° para K é " + calculo, 20, 150 );
    	// body...
    }
     
     if(c == 2){

     	Fahrenheit();
     } 
     
    function kelvin (){

    	var k1 = parseInt(prompt(" Qual valor em kelvin?"));
    	var string1 = '273,15';
    	 var numero1 = parseFloat(string1.replace (',', '.'));

    	 
    	  brush.font ="15x time news roman"
    	   brush.fillStyle = "purple"
    	    brush.fillText(" Transformação de K para C° é " + (k1 - numero1).toFixed(2), 20, 150);


    }

    if(c == 3){

    	kelvin();
    }

    function inverso1 (){

    	var f1 = parseInt(prompt("Qual valor de Fahrenheit?"));
    	 var calculo = ((f1 - 32) * 5) /9;
    	  brush.font ="15x time news roman"
           brush.fillStyle = "orange";
            brush.fillText(" Transformação de F° para C° é " + calculo, 20, 150 );

    }

    if (c == 4) {

    	inverso1();
    }
		    
    function inverso2 (){

    	var k2 = parseInt(prompt(" Qual valor em kelvin?"));
    	 var string2 = "273,15";
    	  var numero2 = parseFloat(string2.replace(',', '.'));

    	  brush.font ="15x time news roman"
           brush.fillStyle = "brow";
            brush.fillText(" Transformação de K para F° é " + ((((k2 - numero2) * 9) / 5) + 32).toFixed(2) , 20, 150 );

    }	
	
	if(c == 5){

		inverso2();
	}	


	   






</script>
