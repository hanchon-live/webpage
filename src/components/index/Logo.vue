<template>
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
</template>

<style lang="scss" scope>
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
import {gsap} from 'gsap';
export default {
    name:'Logo',
    activate() {
    gsap.from(".text h1", {
        duration: 1.5,
        delay: 1,
        y: "100%",
        ease: "expo.inOut",
    });

    gsap.from(".text h3", {
        duration: 1.5,
        delay: 1.2,
        y: "100%",
        ease: "expo.inOut",
    });

    gsap.from(".text p", {
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
    }
}
</script>