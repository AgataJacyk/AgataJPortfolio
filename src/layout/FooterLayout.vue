<template>
  <footer>
    <svg
      viewBox="0 -20 700 110"
      width="100%"
      height="110px"
      preserveAspectRatio="none"
    >
      <path
        transform="translate(0, -20)"
        d="M0,10 c80,-22 240,0 350,18 c90,17 260,7.5 350,-20 v50 h-700"
        fill="#FF0460"
      />
      <path
        d="M0,10 c80,-18 230,-12 350,7 c80,13 260,17 350,-5 v100 h-700z"
        fill="#ffb0a6"
      />
    </svg>
    <div class="sprinkles">
      <h2>Contact</h2>
      <p>tel. 661-470-335</p>
      <p>e-mail: agatajacyk.webdeveloper@gmail.com</p>
      <p>@Copyright Agata J</p>
      <div class="social"><Git /><LinkedIn /></div>
    </div>
  </footer>
</template>

<script>
import Git from "../components/icons/IconGit.vue";
import LinkedIn from "../components/icons/IconLinkedIn.vue";

export default {
  components: {
    Git,
    LinkedIn,
  },
};
</script>

<style lang="scss" scoped>
.sprinkles {
  bottom: 20px;
  z-index: 0;
  background-color: #ffb0a6;
  padding-bottom: 3rem;
  margin-top: -5rem;
}

.social {
  display: flex;
  justify-content: start;
  padding: 1% 3%;
  width: 20%;
  margin: 0 0 0 16px;

  a {
    width: 50%;
    padding: 0 10%;
  }
}

footer {
  width: 100%;
  height: 150px;
  margin-bottom: 0;
  margin-top: -2rem;
  padding-bottom: 0;
  z-index: 10;
}

p {
  margin: 0 0 0 16px;
}
</style>
