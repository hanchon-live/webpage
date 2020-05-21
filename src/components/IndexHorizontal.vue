<template>
    <div class="wrapper">
        <!-- <link href='https://fonts.googleapis.com/css?family=Poppins' rel='stylesheet'> -->

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
            <ul class="ul-header">
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
                <h1><span>Hanchon</span></h1>
                <h2>Live</h2>
                <h3>
                <span>Blockchain <br /> Tools </span>
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

<style lang="scss">
    .ul-header {
        list-style-type: none;
    }

    .media {
        ul {
            position: relative;
            li {
                font-size: 12px;
                font-weight: 600;
                letter-spacing: 2px;
                display: inline-block;
                padding: 0 30px;
                text-transform: uppercase;
            }
        }
    }

    .text {
        h1 {
            text-align: center;
            font-size: 10rem;
            text-transform: uppercase;
            font-weight: 900;
            letter-spacing: -0.9rem;
            position: relative;
        }
        h2 {
            content: "live";
            text-align: center;
            position: relative;
            top: -9rem;
            left: 15.3rem;
            color: #fcc419;
            z-index: -1;
            font-size: 10rem;
            opacity: 1;
        }
        h3 {
            left: 320px;
            font-size: 40px;
            text-transform: uppercase;
            font-weight: 600;
            line-height: 1;
            position: relative;
            overflow: hidden;
            height: 80px;
            text-align: left;
        }
        p {
            text-align: center;
            width: 600px;
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
    @media screen and (max-width: 800px) {
    .text {
        h1 {
                font-size:8rem;
                letter-spacing: -0.7rem;
        }
        h2{
            font-size:8rem;
            letter-spacing: -0.5rem;
            top: -7.5rem;
            left: 11.3rem;
        }
    }
    }
    @media screen and (max-width: 640px) {
    .text {
        h1 {
            font-size:6rem;
            letter-spacing: -0.6rem;
        }
        h2{
            font-size:6rem;
            letter-spacing: -0.3rem;
            top: -5.6rem;
            left: 8.55rem;
        }
    }
    }
    @media screen and (max-width: 470px) {
    .text {
        h1 {
                font-size:5rem;
                letter-spacing: -0.5rem;
        }
        h2{
            font-size:5rem;
            letter-spacing: -0.25rem;
            top: -5rem;
            left: 7.1rem;
        }
    }
    }
    @media screen and (max-width: 400px) {
    .text {
        h1 {
            font-size:4rem;
            letter-spacing: -0.35rem;
        }
        h2{
            font-size:4rem;
            letter-spacing: -0.25rem;
            top: -4rem;
            left: 5.65rem;
        }
    }
    }
</style>

<script>
export default {
    
}
</script>