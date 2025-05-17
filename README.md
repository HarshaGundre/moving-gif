<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Moving Video</title>
    <style>
        html, body {
            height: 100%;
            margin: 0;
            padding: 0;
        }

        body {
            background-image: url("https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRi44cDwbgAOfERYg22Yj0VMepevDFiq8bWsw&s");
            background-size: cover;
            background-repeat: no-repeat;
            background-position: center center;
            background-attachment: fixed;
            overflow: hidden;
        }

        h1 {
            text-align: center;
            color: white;
            padding-top: 20px;
        }

        @keyframes move {
            0% {
                transform: translateX(-100%);
            }
            100% {
                transform: translateX(100vw);
            }
        }

        .moving-gif {
            position: absolute;
            animation: move 10s infinite linear;
        }

        .moving-gif.cheetah {
            top: 300px;
        }

        .moving-gif.lion {
            top: 250px;
            animation-delay: 3s;
            left:-200px;
        }

        .moving-gif.tiger {
            top: 200px;
            animation-delay: 2s;
            left:-100px;
        }
    </style>
</head>
<body>
    <h1>GIFs Moving Left to Right</h1>
    <img class="moving-gif cheetah" src="cheetah run.gif" width="300" height="300" alt="Moving cheetah">
    <img class="moving-gif lion" src="lion running.gif" width="300" height="300" alt="Moving lion">
    <img class="moving-gif tiger" src="tiger running.gif" width="300" height="300" alt="Moving tiger">
</body>
</html>
