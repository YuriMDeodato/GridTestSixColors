<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>css grid</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="wrapper ">
        <div class="box um">um</div>
        <div class="box dois">dois</div>
        <div class="box tres">três</div>
        <div class="box quatro">quatro</div>
        <div class="box cinco">cinco</div>
        <div class="box seis">seis</div>
     </div>

//AND CSS 

*{
    font-family: Arial, Helvetica, sans-serif;
    border: 0;
    margin: 0;

    
}
.box{
    background-color:tomato;
    border: 2px solid black;
    text-align: center;
} 
.um{
    background-color:rgb(123, 255, 71);
    grid-area: um;

}
.dois{
    background-color:rgb(71, 120, 255);
    grid-area: dois;
}
.tres{
    background-color:rgb(255, 71, 86);
    grid-area: tres;
}
.quatro{
    background-color:rgb(255, 114, 71);
    grid-area: quatro;
}
.cinco{
    background-color:rgb(71, 227, 255);
    grid-area: roberto;
}

.seis{
    background-color:rgb(255, 71, 194);
    grid-area: seis;
}

.wrapper {
    display: grid;
    /* grid-template-columns: 200px 200px 200px; */
    grid-template-columns: 1fr 1fr 1fr;
    grid-template-rows: 20vh 40vh 40vh;
    grid-template-areas: 
    "um dois tres"
    "quatro quatro quatro"
    "roberto seis seis";
  }
