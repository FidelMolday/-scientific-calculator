o<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>calculator</title>
   <style >
     *{
    margin: 0;
    padding: 0;
    font-family: 'poppins',sans-serif;
    box-sizing: border-box;

}
.container{
    width: 100%;
    height: 100vh;
    background: #4d1876;
    align-items: center;display: flex;
    justify-content: center;
    display: inline-flexbox;
}
.calculator{
    background: #3a4452;
    padding: 20px;
    border-radius: 10px;
}
.calculator form input{
    border: 0;
    outline: 0;
    width: 60px;
    
    height: 70px;
    border-radius: 10px;
    box-shadow: -8px -8px 15px rgb(255,255 255, 0.1) 5px 5px 15px rgb(0, 0, 0, 0.2);
    font-size: 20px;
    color: #b22727;
    cursor: pointer;
    margin: 10px;

}
.jibu{
    display: flex;
    border: 220px;
    justify-content: flex-end;
    margin: 40px 0;
}
.jibu input{
    text-align: right;
    flex: 1;
    font-size: 45px;
    border: 220px;
    width: 320px;
    background-color: #68129e;
    box-shadow: none;
}
form input.egual{
 width: 145px;   
}

   </style>
</head>
<body>
    <div class="container">
  <div  class="calculator">
    
    <form>
        <div>
            <input class="jibu" id="display1" type="text" name="display" maxlength="50" size="35" width="320px">
        </div>
        <div>
            <input type="button" value="AC" onclick="display.value='' ">
            <input type="button" value="DE"onclick="display.value= display.value.toString().slice(0,-1)">
            <input type="button" value="." onclick="displ.value='.'">
            <input type="button" value="\" onclick="display.value='/'">
        </div>
        <div>
            <input type="button" value="7" onclick="display.value+='7' ">
            <input type="button" value="8"onclick="display.value+='8' ">
            <input type="button" value="9"onclick="display.value+='9' ">
            <input type="button" value="*"onclick="display.value+='*' ">
        </div>
      
        <div>
            <input type="button" value="4"onclick="display.value+='4' ">
            <input type="button" value="5"onclick="display.value+='5' ">
            <input type="button" value="6"onclick="display.value+='6' ">
            <input type="button" value="-"onclick="display.value+='-' ">
        </div>
        <div>
            <input type="button" value="1"onclick="display.value+='1' ">
            <input type="button" value="2"onclick="display.value+='2' ">
            <input type="button" value="3"onclick="display.value+='3' ">
            <input type="button" value="+"onclick="display.value+='+' ">
        </div>
        <div>
            <input type="button" value="00"onclick="display.value+='00' ">
            <input type="button" value="0"onclick="display.value+='0' ">
            <input type="button" value="="  onclick="display.value=eval(display.value)" class="egual">
           
        </div>
    </form>
  </div>  
</body>
</html>
