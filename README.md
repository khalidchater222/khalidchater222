- 👋 Hi, I’m @khalidchater222
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
khalidchater222/khalidchater222 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
<!DOCTYPE html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="cuub.css">
    <title>Document</title>
</head>
<body>
    <div class="cube">
        <div class="top"></div>
        <div>
            <span style="--i :0;"></span>
            <span style="--i :1;"></span>
            <span style="--i :2;"></span>
            <span style="--i :3;"></span>
        </div>

    </div>
</body>
</html>
--> css
{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
body{
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    background: #050505;
}
.cube{
    position: relative;
    width: 300px;
    height: 300px;
    transform-style: preserve-3d;
    transform: rotateX(-30deg);
    animation: animate 4s linear infinite;
}
@keyframes animate
{
    0%
    {
        transform: rotateX(-50deg) rotateY(0deg) rotateZ(40DEG);
    }
    100%
    {
        transform:rotateX(-50deg) rotateY(460deg) rotateZ(40deg);

    }
}
.cube div {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    transform-style: preserve-3d;
}
.cube div span{
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background:linear-gradient(#151515, #1362a7);
    transform: rotateY(calc(90deg * var(--i))) translatez(150px);
}
.top
{
    position:absolute;
    top: 0;
    left: 0;
    width: 300px;
    height: 300px;
    background:rgb(165, 20, 20);
    transform: rotateX(90deg) translateZ(200px);
    
}
.top::before
{
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 300px;
    height: 300px;
    background: rgb(12, 139, 170);
    transform: translateZ(-400px);
    filter: blur(25px);
    box-shadow: 0 0 120px rgba(29, 198, 29, 0.2),
    0 0 200px rgba(29, 198, 29, 0.2),
    
    
    ;
}
