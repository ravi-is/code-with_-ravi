# code-with_-ravi
MSD Profile Card
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title> Simple Profile Card | @codeing.gman </title>
    <link rel="stylesheet" href="style1.css">
</head>

<body>
    <div class="container">
        <div class="card">
            <div class="circle">
                <div>07</div>
            </div>
            <div class="content">
                <h2 class="title">MS DHONI</h2>
                <p>Never doubt the eagle's eye, the leopard's movement and Dhoni's speed!
                </p>
                <p>बाज की नजर, चीते की चाल और धोनी की रफ्तार पर कभी संदेह नहीं करते!</p>
                <p class="righttext">- Thank you</p>
            </div>
        </div>
    </div>
</body>

</html>
@import url('https://fonts.googleapis.com/css2?family=Noto+Sans+JP&display=swap');
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Noto Sans JP', sans-serif;
}

.container {
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100vh;
    background: #ffe6e6;
}

.card {
    height: 400px;
    width: 300px;
    background: #fff;
    z-index: 0;
    border-radius: 20px;
    position: relative;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.15);
}

.card .circle {
    height: 100%;
    border-radius: 20px;
    color: #fff;
    font-weight: 800;
    background-image: url("https://i.pinimg.com/originals/0f/eb/37/0feb371deaa68849765089ba1f00a48e.jpg");
    /* background-size: 120% 120%; */
    animation: 3s circleanimation forwards;
}

@keyframes circleanimation {
    0% {
        background-image: url("https://i.pinimg.com/originals/0f/eb/37/0feb371deaa68849765089ba1f00a48e.jpg");
        background-size: 120% 120%;
        clip-path: circle(800px at center 200px);
    }
    50% {
        background-image: url("https://i.pinimg.com/originals/0f/eb/37/0feb371deaa68849765089ba1f00a48e.jpg");
        background-size: 100% 100%;
    }
    100% {
        background: rgb(255, 86, 71);
        clip-path: circle(250px at center -125px);
    }
}

.circle div {
    font-size: 4em;
    text-align: center;
}

.content {
    z-index: -1;
    position: absolute;
    top: 140px;
    width: 100%;
    color: black;
}

.title {
    font-size: 32px;
    text-align: center;
}

.content p {
    margin-top: 10px;
    padding: 0 20px;
    text-align: justify;
}

.righttext {
    text-align: right !important;
}