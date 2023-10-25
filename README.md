<!DOCTYPE html>
<html>

    <head>
        <meta charset="utf-8">
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <title>Calculator</title>
        <style type="text/css">
            .calc {
                background-color: darkmagenta;
                height: 420px;
                width: 415px;
                margin: 10% 30%;
                border-radius: 250px;
                padding: 50px 0px 0px 150px;
                box-shadow: 0px 0px 10px rgb(248, 247, 248);
            }

            Input {
                width: 50px;
                height: 50px;
                background-color: black;
                color: white;
                border: 1px solid white;
                border-radius: 25px;
                margin: 4px;
                font-size: 18px;
                transition-duration: 0.5s;
            }



            .operator {

                background-color: orange;
                color: black;
                font-size: 20px;
                font-weight: bold;
                border: 1px solid black;
            }

            .ac {
                width: 112px;
                margin-right: 5px;
                color: black;
                border: 1px solid black;
                font-size: 20px;
                font-weight: bold;

            }

            .ac:hover {
                transform: scale(0.9);
            }

            .op {
                height: 70px;
                width: 230px;


                background-size: cover;
                box-shadow: 0px 0px 2px grey;
                color: rgb(247, 242, 242);
                font-size: 30px;
                text-align: right;
                border: 2px solid black;

            }

            #allclear {
                background-color: orange;
            }

            .operator:hover {
                transform: scale(0.9);
            }

            Input [type="button"]:hover {
                transform: scale(0.9s);
                box-shadow: 0px 0px 5px orange;
                color: lightgreen;
            }

            .bd {
                background-color: black;
                background-size: cover;
                background-image: url(mini.jpg);
            }
        </style>
    </head>


    <body class="bd">
        <div class="calc">
            <form>

                <div>
                    <input type="text" placeholder="MINI COOPER" name="op" disabled class="op">
                </div>
                <div>
                    <input type="button" value="AC" onclick="op.value=''" class="ac" id="allclear">
                    <input type="button" value="C" onclick="op+= '' " class="operator">
                    <input type="button" value="%" onclick="op.value+='%' " class="operator">
                </div>
                <div>
                    <input type="button" value="7" onclick="op.value+='7' ">
                    <input type="button" value="8" onclick="op.value+='8' ">
                    <input type="button" value="9" onclick="op.value+='9' ">
                    <input type="button" value="+" onclick="op.value+='+' " class="operator">
                </div>
                <div>
                    <input type="button" value="4" onclick="op.value+='4' ">
                    <input type="button" value="5" onclick="op.value+='5' ">
                    <input type="button" value="6" onclick="op.value+='6' ">
                    <input type="button" value="-" onclick="op.value+='-' " class="operator">
                </div>
                <div>
                    <input type="button" value="1" onclick="op.value+='1' ">
                    <input type="button" value="2" onclick="op.value+='2' ">
                    <input type="button" value="3" onclick="op.value+='3' ">
                    <input type="button" value="*" onclick="op.value+='*'" class="operator">
                </div>
                <div>
                    <input type="button" value="." onclick="op.value+='.' ">
                    <input type="button" value="0" onclick="op.value+='0' ">
                    <input type="button" value="=" onclick="op.value=eval(op.value)" class="operator">
                    <input type="button" value="/" onclick="op.value+='/' " class="operator">
                </div>
            </form>
        </div>

    </body>

</html>
