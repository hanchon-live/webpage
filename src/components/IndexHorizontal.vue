<template>
    <div class="wrapper">
        <!-- <link href='https://fonts.googleapis.com/css?family=Poppins' rel='stylesheet'> -->

        <!-- OVERLAY
        =============================== -->
        <!-- <div class="overlay first"></div>
        <div class="overlay second"></div>
        <div class="overlay third"></div> -->
        <Loading />
        
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
        
        <Logo />
        
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
</style>

<script>
import Loading from './index/Loading.vue'
import Logo from './index/Logo.vue'
export default {
    name:'IndexHorizontal',
    components: {
        Loading,
        Logo
    },
    mounted() {
        Loading.activate()
        Logo.activate()
    }
    
}
</script>