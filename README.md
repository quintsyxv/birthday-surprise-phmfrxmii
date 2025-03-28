# birthday-surprise-phmfrxmii
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday!</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #fdd;
            flex-direction: column;
            text-align: center;
        }
        .cake {
            position: relative;
            width: 200px;
            height: 150px;
            background: pink;
            border-radius: 10px;
        }
        .candle {
            position: absolute;
            top: -40px;
            left: 50%;
            width: 10px;
            height: 40px;
            background: red;
            transform: translateX(-50%);
        }
        .flame {
            position: absolute;
            top: -20px;
            left: 50%;
            width: 15px;
            height: 20px;
            background: orange;
            border-radius: 50%;
            transform: translateX(-50%);
        }
    </style>
</head>
<body>
    <h1>🎉 สุขสันต์วันเกิด! 🎂</h1>
    <p>คลิกที่เค้กเพื่อเป่าเทียน!</p>
    <div class="cake" onclick="blowCandle()">
        <div class="candle">
            <div class="flame" id="flame"></div>
        </div>
    </div>
    <script>
        function blowCandle() {
            document.getElementById("flame").style.display = "none";
            alert("เย่! เทียนดับแล้ว สุขสันต์วันเกิดนะ!");
        }
    </script>
</body>
</html>
