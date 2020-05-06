<head>
    <meta charset="UTF-8">
    <title>Formas</title>
    <link href="css/stils.css" rel="stylesheet" type="text/css">
</head>
<body>
    <h1>Formas un ievadlauku piemērs</h1>
    <form>
        <p>Šodienas datums <input name="datums"></p>
        <p>Ja gribi uzzināt šodienas datumu, spied pogu DATUMS 
            <input onclick="datums.value=new Date();" name="poga" value="DATUMS" type="button">
        </p>
        <p>Ja gribi izdzēst datuma lodziņa saturu, spied pogu RESET
            <input value="RESET" type="reset">
        </p>
    </form>
    <form>
        <div>1.skaitlis<input type="text" name="sk1"> </div>
        <div>
            <input value="X" name="reiz" onclick="rez.value=sk1.value*sk2.value" type="button">
        </div>
        <div>
            <input value="+" name="plus" onclick="rez.value=sk1.value + sk2.value" type="button">
        </div>
        <div>
            <input value="-" name="mīnus" onclick="rez.value=sk1.value-sk2.value" type="button">
        </div>
        <div>
            <input value="/" name="dalīt" onclick="rez.value=sk1.value/sk2.value" type="button">
        </div>
        <div>2.skaitlis<input type="number" name="sk2"> </div>
        <hr>
        <div>Rezultāts<input name="rez"> </div>
    </form>

<head>
    <meta charset="UTF-8">
    <script>
    function krasot(){
        var kr=document.getElementById("krasa").value;
        document.getElementById("fons").style="background-color:"+kr;
    }
    </script>
</head>
<form>
  <div id="fons" style="background-color:lightgrey">Izvēlies krāsu!</div>
  <input type="color" id="krasa" value="#00ff00" onclick="krasot();">
 
</form>
</body>
</html>
