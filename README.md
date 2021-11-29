<!DOCTYPE html>
<html lang="en">
<head>
     <meta charset="UTF-8">
     <meta http-equiv="X-UA-Compatible" content="IE=edge">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <title>Document</title>
</head>
<script>
    function DisplayInput() {
        var  nWNumber = document.getElementById("wnum").value;
        alert(nWNumber)
    }
    function isEven(num) {
        if (num % 2 == 0)
             return ture;
        else
             return false;
    }
    function onBtnClkSubmit() {
        let inputVal = document.getWElemenById("wnum").value;
        var A = isEven(inputVal);
        if (A){
            document.getWElemenById("result").innerHTML = inputVal + "是偶數";
        }
        else{
            document.getWElemenById("result").innerHTML = inputVal + "是奇數";
        }    

    }
    </script>
    <body>
    <label for="wnum"> Please input a whole number</label>
    <input type="text" id = "wnum" name = "wnum"> <br><br>
    <button type="button" onclick = "onBtnClkSubmit()" >Submit</button>

    <p id = "result"> display result here... </p>
    </body>
    </html>
