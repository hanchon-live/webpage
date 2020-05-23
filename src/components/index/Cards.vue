<template>
<b-container fluid>

<b-row>

<b-col cols="12" md="4">
  <b-card
    class="mb-2 title card"
  >
  <b-card-title>
    <ion-icon name="cube-outline" class="thin"></ion-icon>
    <h1>
    Testnet
    </h1>
  </b-card-title>
    <b-card-text>
        <h4>
         Utils running on top of the Bitcoin Cash Testnet (TBCH).
         </h4>
    </b-card-text>

    <div class="row center">
        <div class="col-12">
            <a href="#" class="btn btn-sm animated-button thar-three">Faucet</a>
            <!-- <b-button class="button" href="#" variant="primary"></b-button> -->
        </div>
        <div class="col-12">
            <a href="#" class="btn btn-sm animated-button thar-three">Explorer</a>
            <!-- <b-button class="button" href="#" variant="primary">Explorer</b-button> -->
        </div>
        <div class="col-12">
            <a href="#" class="btn btn-sm animated-button thar-three">Run your own Testnet</a>
            <!-- <b-button class="button" href="#" variant="primary">Run your own Testnet</b-button> -->
        </div>
    </div>
  </b-card>
</b-col>

</b-row>
</b-container>

</template>

<script>
  export default {

  };
</script>


<style scope>
h1 {
    margin-top: 1rem;
}
h4 {
    font-size: 1.3rem;
}
.thin {
  --ionicon-stroke-width: 1.5rem;
  font-size: 7rem;
  border-radius: 20px;
  margin-top: -60rem;
  background-color: #fcc419;
  box-shadow: 7px 7px 20px black;

}
.center {
    text-align: center;
}
.button {
    margin: 0.5rem;
}
.title {
    color:white;
}
.card {
    /* background: #2c303a; */
    background:#2c3e50;
    padding: 1.5rem 1.5rem 2rem;
    margin: 2rem 2rem;
    border-radius: 10px;
    position: relative;
    z-index: 1;
    box-shadow: 5px 5px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);

}

/* Global Button Styles */
a.animated-button:link, a.animated-button:visited {
    position: relative;
    display: block;
    margin: 30px auto 0;
    padding: 14px 15px;
    color: #fff;
    font-size:14px;
    font-weight: bold;
    text-align: center;
    text-decoration: none;
    text-transform: uppercase;
    overflow: hidden;
    letter-spacing: .08em;
    border-radius: 0;
    text-shadow: 0 0 1px rgba(0, 0, 0, 0.2), 0 1px 0 rgba(0, 0, 0, 0.2);
    -webkit-transition: all 1s ease;
    -moz-transition: all 1s ease;
    -o-transition: all 1s ease;
    transition: all 1s ease;
}
a.animated-button:link:after, a.animated-button:visited:after {
    content: "";
    position: absolute;
    height: 0%;
    left: 50%;
    top: 50%;
    width: 150%;
    z-index: -1;
    -webkit-transition: all 0.75s ease 0s;
    -moz-transition: all 0.75s ease 0s;
    -o-transition: all 0.75s ease 0s;
    transition: all 0.75s ease 0s;
}
a.animated-button:link:hover, a.animated-button:visited:hover {
    color: #FFF;
    text-shadow: none;
}
a.animated-button:link:hover:after, a.animated-button:visited:hover:after {
    height: 450%;
}
a.animated-button:link, a.animated-button:visited {
    position: relative;
    display: block;
    margin: 30px auto 0;
    padding: 14px 15px;
    color: #fff;
    font-size:14px;
    border-radius: 0;
    font-weight: bold;
    text-align: center;
    text-decoration: none;
    text-transform: uppercase;
    overflow: hidden;
    letter-spacing: .08em;
    text-shadow: 0 0 1px rgba(0, 0, 0, 0.2), 0 1px 0 rgba(0, 0, 0, 0.2);
    -webkit-transition: all 1s ease;
    -moz-transition: all 1s ease;
    -o-transition: all 1s ease;
    transition: all 1s ease;
}

a.animated-button.thar-three {
    color: #fff;
    cursor: pointer;
    display: block;
    position: relative;
    border: 2px solid #fcc419;
    transition: all 0.4s cubic-bezier(0.42, 0, 0.58, 1);
}
a.animated-button.thar-three:hover {
    color: #000 !important;
    background-color: transparent;
    text-shadow: nthree;
}
a.animated-button.thar-three:hover:before {
    left: 0%;
    right: auto;
    width: 100%;
}
a.animated-button.thar-three:before {
    display: block;
    position: absolute;
    top: 0px;
    right: 0px;
    height: 100%;
    width: 0px;
    z-index: -1;
    content: '';
    color: #000 !important;
    background: #fcc419;
    transition: all 0.4s cubic-bezier(0.42, 0, 0.58, 1);
}
</style>