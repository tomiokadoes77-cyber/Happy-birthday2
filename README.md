<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tanishka Birthday</title>

    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet"
        href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    <link
        href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@500;700&family=Poppins:wght@400;600&display=swap"
        rel="stylesheet">
    <script src="https://code.jquery.com/jquery-3.7.1.min.js"></script>
</head>

<body>
    <div id="wrapper">

        <div class="flag__birthday">
            <img src="./images/1.png" width="350" class="flag__left">
            <img src="./images/1.png" width="350" class="flag__right">
        </div>

        <div class="content">
            <div class="left">
                <div class="title">
                    <h1 class="happy">
                        <span style="--t:4s">H</span>
                        <span style="--t:4.2s">a</span>
                        <span style="--t:4.4s">p</span>
                        <span style="--t:4.6s">p</span>
                        <span style="--t:4.8s">y</span>
                    </h1>

                    <h1 class="birthday">
                        <span style="--t:5s">B</span>
                        <span style="--t:5.2s">i</span>
                        <span style="--t:5.4s">r</span>
                        <span style="--t:5.6s">t</span>
                        <span style="--t:5.8s">h</span>
                        <span style="--t:6s">d</span>
                        <span style="--t:6.2s">a</span>
                        <span style="--t:6.4s">y</span>
                    </h1>

                    <div class="hat">
                        <img src="./images/hat.png" width="130">
                    </div>
                </div>

                <div class="date__of__birth">
                    <span></span>
                </div>

                <div class="btn">
                    <button id="btn__letter">
                        <div class="mail">
                            Click Here Tanishka
                            <i class="fa-regular fa-envelope"></i>
                        </div>
                    </button>
                </div>
            </div>

            <div class="right">
                <div class="box__account">
                    <div class="image">
                        <img src="./images/unnamed.png">
                    </div>

                    <div class="name">
                        <i class="fa-solid fa-heart"></i>
                        <span>Dear Tanishka</span>
                        <i class="fa-solid fa-heart"></i>
                    </div>

                    <div class="balloon_one">
                        <img src="./images/balloon1.png" width="100">
                    </div>
                    <div class="balloon_two">
                        <img src="./images/balloon2.png" width="100">
                    </div>
                </div>

                <div class="cricle">
                    <div class="text__cricle">
                        <span style="--i:1">h</span>
                        <span style="--i:2">a</span>
                        <span style="--i:3">p</span>
                        <span style="--i:4">p</span>
                        <span style="--i:5">y</span>
                        <span style="--i:6">-</span>
                        <span style="--i:7">b</span>
                        <span style="--i:8">i</span>
                        <span style="--i:9">r</span>
                        <span style="--i:10">t</span>
                        <span style="--i:11">h</span>
                        <span style="--i:12">d</span>
                        <span style="--i:13">a</span>
                        <span style="--i:14">y</span>
                        <span style="--i:15">-</span>
                    </div>
                    <i class="fa-solid fa-heart"></i>
                </div>
            </div>
        </div>

        <!-- MAIL BOX -->
        <div class="boxMail">
            <i class="fa-solid fa-xmark"></i>

            <div class="boxMail-container">
                <div class="card1">
                    <div class="userImg">
                        <img src="images/unnamed.png">
                    </div>
                    <h4 class="username">To: Tanishka 💖</h4>
                    <h3>Happy Birthday</h3>
                    <img src="cute1.png">
                </div>

                <div class="card2">
                    <div class="card2-content">
                        <h3>To You!</h3>

                        <h2>
                            Happy Birthday 🥳🎂  
                            From the moment you slowly became a part of my life,
                            something inside me changed.  
                            I didn’t realize it at first, but day by day you grew
                            closer to my heart.  

                            You matter to me more than you know.  
                            I wish I could take away every worry that ever made
                            you feel alone — but until then, just know I’m always
                            here for you 🤍  

                            You can talk to me anytime, about anything —
                            especially the things you don’t say out loud.  
                            May this year bring you peace, smiles, and everything
                            your heart quietly wishes for.  

                            Stay happy, stay you 😌  
                            Happy Birthday 🎈🎂
                        </h2>

                        <img src="cute2.png">
                    </div>
                </div>
            </div>
        </div>
    </div>

<script>
    let datetxt = "15 February";
    let datatxtletter = "My love. You are someone very special to me. I silently thank the universe for bringing you into my life. On your birthday, I wish you happiness, good health, and endless smiles. I hope we get to celebrate many more days like this together. Happy Birthday 💕";

    let charArrDate = datetxt.split('');
    let currentIndex = 0;
    let date__of__birth = document.querySelector(".date__of__birth span");

    setInterval(() => {
        if (currentIndex < charArrDate.length) {
            date__of__birth.textContent += charArrDate[currentIndex++];
        }
    }, 100);

    let mailBox = document.querySelector('.mail');
    let boxmail = document.querySelector('.boxMail');
    let close = document.querySelector('.fa-xmark');

    mailBox.onclick = () => boxmail.classList.add('active');
    close.onclick = () => boxmail.classList.remove('active');
</script>

</body>
</html>

