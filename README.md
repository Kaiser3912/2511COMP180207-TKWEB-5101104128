<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Image Hover</title>
    <style>
        body {
            background-color: rgb(39, 35, 35);
            font-family: dejaVu Sans, sans-serif;
        }
        h1 {
            color: white;
            text-align: center;
        }
        .box {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            align-items: center;
            width: 90%;
        }
        .image {
            width: 270px;
            height: 180px;
            overflow: hidden;
            border-radius: 10px;
            position: relative;
            display: inline-block;
            margin: 20px;
        }
        .image img {
            width: 100%;
            height: 100%;
            transition: all 0.5s;
            object-fit: cover;
        }
        .image:hover img {
            transform: scale(1.2);
            filter: brightness(90%);
        }
        .edit {
            position: absolute;
            bottom: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.6);
            color: white;
            text-align: center;
            line-height: 40px;
            font-size: 18px;
            opacity: 0;
            transition: all 0.5s;
            justify-content: center;
            align-items: center;
            display: flex;
        }
        .image:hover .edit {
            opacity: 1;
        }
    </style>
</head>
<body>
    <h1>Landscape</h1>
    <div class="box">
        <div class="image">
            <img src="hinh/19.jpg" alt="SunRise" width="300" height="400">
            <div class="edit">SunRise</div>
        </div>
        <div class="image">
            <img src="hinh/21.jpg" alt="Forest" width="300" height="400">
            <div class="edit">Forest</div>
        </div>
        <div class="image">
            <img src="hinh/18.jpg" alt="Moon" width="300" height="400">
            <div class="edit">Moon</div>
        </div>
        <div class="image">
            <img src="hinh/lake.jpg" alt="Lake" width="300" height="400">
            <div class="edit">Lake</div>
        </div>
        <div class="image">
            <img src="hinh/20.jpg" alt="Rain" width="300" height="400">
            <div class="edit">Rain</div>
        </div>
    </div>
</body>
</html>
