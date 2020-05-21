<template>
    <div class="wrapper">
        <!-- <link href='https://fonts.googleapis.com/css?family=Poppins' rel='stylesheet'> -->
        <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@500;600;700;900&amp;display=swap" rel="stylesheet">
        <script type="module" src="https://unpkg.com/ionicons@5.0.0/dist/ionicons/ionicons.esm.js"></script>

            <!-- OVERLAY
            =============================== -->
            <div class="overlay first"></div>
            <div class="overlay second"></div>
            <div class="overlay third"></div>
            
            <!-- NAVBAR 
            =============================== -->
            <div class="navbar">
                <div class="menu">
                <!-- <ion-icon name="menu-outline"></ion-icon>
                </div>
                <div class="lang">Eng</div>
                <div class="search">
                <ion-icon name="search-outline"></ion-icon> -->
                </div>
            </div>
            
            <!-- SOCIAL MEDIA 
            =============================== -->
            <div class="media">
                <ul>
                <li>twitch</li>
                <li>twitter</li>
                <li>discord</li>
                <li>docs</li>
                <li>github</li>
                </ul>
            </div>
            
            <!-- TEXT 
            =============================== -->
            <div class="text">
                    <h1><span class="hide--text">Hanchon</span></h1>
                    <h2>Live</h2>
                    <h3>
                    <span class="hide--text">Blockchain <br /> Tools </span>
                    </h3>
                    <p>
                    <span class="hide--text">
                       Collection of useful programs and scripts to interact with blockchains.
                    </span>
                    </p>
                </div>
            
            <!-- SPONSOR 
            =============================== -->
            <!-- <div class="sponsor">
                <img src="https://www.dropbox.com/s/6alm9s749j5z6e6/sponsor-logo.png?raw=1" alt="">
                <p>official sponsor</p>
            </div> -->
            
            <!-- DISTORTION 
            =============================== -->
            <div class="distortion">
                <div class="col">
                    <div class="row">
                        <h3>Bitcoin cash Testnet:</h3>
                    </div>
                    <div class="row">
                        <ul>
                            <li>Faucet</li>
                            <li>Explorer</li>
                            <li>Run your own Testnet</li>
                        </ul>
                    </div>

                    <div class="row">
                        <h3>HanchonD</h3>
                    </div>
                    <div class="row">                        
                        <ul>
                            <li>Github</li>
                            <li>Docker</li>
                        </ul>
                    </div>

                    <div class="row">
                        <h3>Codes:</h3>
                    </div>
                    <div class="row">
                        <ul>
                            <li>Faucet (nodejs)</li>
                            <li>Upload files (python)</li>
                            <li>Tx sender (nodejs)</li>
                            <li>Forks watchet (nodejs)</li>
                        </ul>
                    </div>

                </div>
                <!-- <img src="https://www.dropbox.com/s/827kuldqiqfpqlg/02.png?raw=1" alt=""> -->
                <!-- <img src="../assets/background.png" alt=""> -->
            </div>

        </div>

</template>

<script>
import {gsap} from 'gsap';
export default {
mounted() {
    /* NAVBAR */
    gsap.from(".navbar div", {
    duration: 1.5,
    delay: 1.5,
    opacity: 0,
    y: "20",
    ease: "expo.inOut",
    stagger: 1
    });

    /* MEDIA */
    gsap.from(".media ul li", {
    duration: 1.5,
    delay: 1.5,
    stagger: 0.08,
    opacity: 0,
    x: "-20",
    ease: "expo.inOut",
    });

    /* TEXT */
    gsap.from(".text h1 .hide--text", {
    duration: 1.5,
    delay: 1,
    y: "100%",
    ease: "expo.inOut",
    });

    gsap.from(".text h3 .hide--text", {
    duration: 1.5,
    delay: 1.2,
    y: "100%",
    ease: "expo.inOut",
    });

    gsap.from(".text p .hide--text", {
    duration: 1.5,
    delay: 1.3,
    y: "200%",
    ease: "expo.inOut",
    });

    gsap.from(".text h2", {
    duration: 1.5,
    delay: 1.5,
    opacity: 0,
    x: "-10000",
    ease: "expo.inOut",
    });

    /* SPONSOR */
    gsap.from(".sponsor img", {
    duration: 1.5,
    delay: 1.5,
    opacity: 0,
    y: "20",
    ease: "expo.inOut",
    });

    gsap.from(".sponsor p", {
    duration: 1.5,
    delay: 1.6,
    opacity: 0,
    y: "20",
    ease: "expo.inOut",
    });

    /* DISTORTION */
    gsap.from(".distortion", {
    duration: 1.5,
    delay: 2,
    opacity: 0,
    y: "20",
    ease: "expo.inOut",
    });

    /* OVERLAY */
    gsap.to(".first", {
    duration: 1.5,
    delay: 0.5,
    top: "-100%",
    ease: "expo.inOut",
    });

    gsap.to(".second", {
    duration: 1.5,
    delay: 0.6,
    top: "-100%",
    ease: "expo.inOut",
    });

    gsap.to(".third", {
    duration: 1.5,
    delay: 0.7,
    top: "-100%",
    ease: "expo.inOut",
    });
}
}

</script>

<style lang="scss">
    * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    }

    body {
    font-family: "Poppins", sans-serif;
    background: #f1f3f5;
    widows: 100%;
    height: 100vh;
    overflow: hidden;
    }

    ul {
    list-style-type: none;
    }

    /* NAVBAR 
    =============================== */
    .navbar {
    display: flex;
    justify-content: space-between;
    height: 80px;
    align-items: center;
    overflow: hidden;
    opacity: 1;
    > div {
        padding: 0 30px;
        font-size: 20px;
    }
    .menu {
        margin-right: auto;
    }
    .lang {
        font-size: 10px;
        font-weight: 600;
        text-transform: uppercase;
    }
    }

    /* SOCIAL MEDIA 
    =============================== */
    .media {
    ul {
        position: absolute;
        bottom: 250px;
        left: -140px;
        transform: rotate(-90deg);
        li {
        font-size: 10px;
        font-weight: 600;
        letter-spacing: 2px;
        display: inline-block;
        padding: 0 30px;
        text-transform: uppercase;
        }
    }
    }

    /* TEXT 
    =============================== */
    .text {
    position: absolute;
    top: 200px;
    left: 100px;
    transform: rotate(-90deg);
    h1 {
        text-align: left;
        font-size: 120px;
        text-transform: uppercase;
        font-weight: 900;
        letter-spacing: -10px;
        position: relative;
        overflow: hidden;
        height: 150px;
        width: 600px;
        .hide--text {
        position: absolute;
        }
    }
    h2 {
        content: "duality";
        position: absolute;
        top: 40px;
        left: -80px;
        color: #fcc419;
        z-index: -1;
        font-size: 150px;
        opacity: 1;
    }
    h3 {
        font-size: 40px;
        text-transform: uppercase;
        font-weight: 600;
        line-height: 1;
        position: relative;
        overflow: hidden;
        height: 80px;
        .hide--text {
        position: absolute;
        }
    }
    p {
        width: 400px;
        font-size: 12px;
        margin-top: 30px;
        font-weight: 500;
        position: relative;
        overflow: hidden;
        height: 100px;
        .hide--text {
        position: absolute;
        }
    }
    }

    /* SPONSOR 
    =============================== */
    .sponsor {
    position: absolute;
    right: 100px;
    bottom: 100px;
    text-align: center;
    img {
        width: 200px;
        opacity: 1;
        transform: rotate(-90deg);
    }
    p {
        margin-top: 20px;
        font-size: 12px;
        text-transform: uppercase;
        font-weight: 900;
        transform: rotate(180deg);
    }
    }

    /* DISTORTION 
    =============================== */
    .distortion {
    display: flex;
    width: 580px;
    height: 720px;
    position: absolute;
    right: 500px;
    bottom: 0;
    }


    /* OVERLAY 
    =============================== */
    .overlay{
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    z-index: 99;
    overflow: hidden;
    &.first{ 
        background: #fcc419;
    }
    &.second{
        background: #fcc419;
        left: 33.33%;
    }
    &.third{
        background: #fcc419;
        left: 66.66%;
    }
    }
</style>