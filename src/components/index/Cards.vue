<template>
  <b-container class="pt-3" fluid>
    <b-row>
      <Card
        :name="cards.testnet.name"
        :subtitle="cards.testnet.subtitle"
        :icon="cards.testnet.icon"
        :buttons="cards.testnet.buttons"
      />
      <Card
        :name="cards.hanchond.name"
        :subtitle="cards.hanchond.subtitle"
        :icon="cards.hanchond.icon"
        :buttons="cards.hanchond.buttons"
      />
      <Card
        :name="cards.socials.name"
        :subtitle="cards.socials.subtitle"
        :icon="cards.socials.icon"
        :buttons="cards.socials.buttons"
      />
    </b-row>
  </b-container>
</template>

<script>
import Card from "./Card.vue";
export default {
  components: {
    Card,
  },
  data: function () {
    return {
      cards: {
        socials: {
          name: "Socials",
          subtitle: "Find me in the web.",
          icon: "chatbox-ellipses-outline",
          buttons: [
            {
              text: "Paolettips (Guides and Tips)",
              dest: "https://paolettips.com",
            },
            {
              text: "github",
              dest: "https://github.com/hanchon",
            },
            {
              text: "twitter",
              dest: "https://twitter.com/gepaoletti",
            },
            {
              text: "twitch",
              dest: "https://www.twitch.tv/elhachon",
            },
          ],
        },
        testnet: {
          name: "Ethermint",
          subtitle: "Utils running on Ethermint testnet network.",
          icon: "cube-outline",
          buttons: [
            {
              text: "Ethermint Testnet Faucet",
              dest: "https://faucet.hanchon.live/",
            },
            {
              text: "Explorer (Coming soon)",
              dest: "#",
            },
            {
              text: "Deploy Faucet Guide",
              dest: "https://paolettips.com/blog/2021/08/26/how-to-deploy-a-ethermint-faucet/",
            },
            {
              text: "Build Ethermint Node",
              dest: "https://paolettips.com/blog/2021/07/30/ethermint-build/",
            },
          ],
        },
        hanchond: {
          name: "Bitcoin Cash",
          subtitle: "Utils for Bitcoin Cash Testnet (TBCH).",
          icon: "hourglass-outline",
          buttons: [
            {
              text: "Run your own testnet",
              dest: "https://docs.hanchon.live/bch-testnet-environment/introduction",
            },
            {
              text: "File hash uploader",
              dest: "https://github.com/hanchon/cash_file_uploader",
            },
          ],
        },
      },
    };
  },
};
</script>


<style scope>
h1 {
  margin-top: 0.2rem;
}
h4 {
  font-size: 1.1rem;
}
.thin {
  --ionicon-stroke-width: 1.5rem;
  font-size: 7rem;
  border-radius: 20px;
  margin-top: -60rem;
  background-color: #fcc419;
  box-shadow: 5px 5px 20px black;
}
.center {
  text-align: center;
}
.button {
  margin: 0.2rem;
}
.title {
  color: white;
}
.card {
  background: #2c3e50;
  padding: 1.5rem 1.5rem 2rem;
  margin: 2rem 2rem;
  border-radius: 10px;
  position: relative;
  z-index: 1;
  box-shadow: 5px 5px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
}
a {
  margin: 0.3rem !important;
}

@media screen and (max-width: 1300px) {
  .thin {
    font-size: 6rem;
  }
  h1 {
    font-size: 2rem;
  }
  h4 {
    font-size: 0.8rem;
  }
}
@media screen and (max-width: 400px) {
  .thin {
    font-size: 5rem;
  }
}
</style>