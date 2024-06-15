<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta
        name="viewport"
        content="width=device-width, initial-scale=1.0, minimum-scale=0.5, maximum-scale=2.0, user-scalable=no,minimal-ui"
    />
    <title>DIY水印相机</title>
    <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
    <style>
        body {
            font-family: 'Microsoft YaHei', Arial, sans-serif;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 115vh;
            margin: 0;
            background-color: #f0f0f0;
        }
        #videoContainer {
            position: relative;
            width: 380px;
            height: 500px; /* Fixed height for video and image */
            overflow: hidden; /* Hide overflow content */
            background-color: black;
        }
        #videoElement, #imageElement {
            position: absolute;
            top: 50%;
            left: 50%;
            width: 100%; /* Always take full width */
            height: auto; /* Adjust height automatically */
            transform: translate(-50%, -50%);
        }
        #watermark {
            position: absolute;
            bottom: 10px;
            left: 10px;
            color: white;
            font-size: 15px;
            font-weight: 500;
            letter-spacing: 0px;
            padding: 5px;
            border-radius: 5px;
        }
        #time {
            background: linear-gradient(to bottom, #5798ff, black);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            font-size: 1.5em;
            font-weight: bold;
            padding-left: 12.8px;
            transform: scaleX(0.8);
        }
        #times {
            padding-left: 3px;
            transform: scaleX(0.8);
            margin-top: -80px;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <div id="videoContainer">
        <video id="videoElement" autoplay playsinline></video>
        <img id="imageElement" style="display:none;">
        <div id="watermark" style="margin-bottom: -16.3px;">
            <img src="bj.png" style="position: initial;width: 380px;margin-bottom: -113.3px;margin-left: -15px;">
            <div id="time"></div>
            <div id="watermarkTextb" style="transform: scaleX(0.9);padding-top: 8px;margin-left: -10px;padding-bottom: 1px;letter-spacing: 0.1px;font-weight: bold;">广东省东莞市虎门镇</div>
            <div id="watermarkTextc" style="padding-bottom: 19px;padding-left: 10px;letter-spacing: 0px;">获取中</div>
            <div id="fw" style="transform: scaleX(0.8);letter-spacing: 0px;margin-left: 303px;font-size: 6.5px;margin-bottom: 0px;font-weight: bold;margin-top: -1.8px;">获取中</div>
        </div>
    </div>
    <div>
        <button id="startCamera">使用相机</button>
        <input type="file" id="uploadImage" accept="image/*">
    </div>
    <div>
        <label for="watermarkInput">A水印:</label>
        <input type="text" id="watermarkInputa" placeholder="A水印">
        <label for="watermarkInput">B水印:</label>
        <input type="text" id="watermarkInputb" placeholder="B水印">
        <label for="watermarkInput">C水印:</label>
        <input type="text" id="watermarkInputc" placeholder="C水印">
        <button id="updateWatermark">更新水印</button>
    </div>
    <br>
    <p>本项目仅供学习参考，请勿非法使用，否则后果自负！</p>
    <script>
        $(document).ready(function () {
            const videoElement = document.getElementById('videoElement');
            const imageElement = document.getElementById('imageElement');
            const watermarka = document.getElementById('time');
            const watermarkb = document.getElementById('watermarkTextb');
            const watermarkc = document.getElementById('watermarkTextc');
            $("#fw").text(generateRandomString(14));
            var currentDate = new Date();
            var hours = ("0" + currentDate.getHours()).slice(-2);
            var minutes = ("0" + currentDate.getMinutes()).slice(-2);
            var formattedTime = hours + ":" + minutes;
            $("#time").text(formattedTime);
            $("#watermarkInputa").val(formattedTime);
            var days = ['星期日', '星期一', '星期二', '星期三', '星期四', '星期五', '星期六'];
            var currentDate = new Date();
            var year = currentDate.getFullYear();
            var month = ("0" + (currentDate.getMonth() + 1)).slice(-2);
            var day = ("0" + currentDate.getDate()).slice(-2);
            var dayOfWeek = days[currentDate.getDay()];
            var formattedDate = year + "." + month + "." + day + " " + dayOfWeek;
            $("#watermarkTextc").text(formattedDate);
            $("#watermarkInputb").val('广东省广州市白云区龙井西路4号');
            $("#watermarkInputc").val(formattedDate);
            $('#startCamera').click(function () {
                $('#imageElement').hide();
                $('#videoElement').show();
                if (navigator.mediaDevices.getUserMedia) {
                    navigator.mediaDevices.getUserMedia({ 
                        video: { facingMode: { exact: "environment" } } 
                    })
                    .then(function (stream) {
                        videoElement.srcObject = stream;
                    })
                    .catch(function (error) {
                        console.log("Something went wrong!", error);
                    });
                }
            });
            $('#uploadImage').change(function (event) {
                $('#videoElement').hide();
                $('#imageElement').show();
                const file = event.target.files[0];
                const reader = new FileReader();
                reader.onload = function (e) {
                    $('#imageElement').attr('src', e.target.result);
                }
                reader.readAsDataURL(file);
            });
            $('#updateWatermark').click(function () {
                watermarka.textContent = $('#watermarkInputa').val();
                watermarkb.textContent = $('#watermarkInputb').val();
                watermarkc.textContent = $('#watermarkInputc').val();
                $("#fw").text(generateRandomString(14));
            });
        });
        function generateRandomString(length) {
            const characters = 'ABCDEFGHIJKMNOPQRSTUVWXYZ0123456789';
            let result = '';
            const charactersLength = characters.length;
            for (let i = 0; i < length; i++) {
                result += characters.charAt(Math.floor(Math.random() * charactersLength));
            }
            return result;
        }
    </script>
</body>
</html>
