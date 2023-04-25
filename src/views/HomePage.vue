<template>
  <section class="welcome">
    <div class="profile">
      <img src="/smiley.png" alt="smiley face" />
    </div>
    <h1>Hello there!</h1>
    <p>
      My name is Agata. This is my portfolio page! Scroll down if you want to
      know me better
    </p>
  </section>
  <Websites></Websites>
  <Designs></Designs>
  <LastPanel></LastPanel>
</template>

<script>
import Designs from "../components/Designs.vue";
import Websites from "../components/Websites.vue";
import LastPanel from "../components/LastPanel.vue";

export default {
  components: {
    Websites,
    Designs,
    LastPanel,
  },
};
</script>

<style lang="scss" scoped>
img {
  width: 150px;
  height: auto;
}
h1,
p {
  margin: 0 auto;
}
p {
  text-align: center;
  width: 50%;
  padding: 0;
}
.profile {
  margin: 0 auto;
  background: #ffb0a6;
  border-radius: 50%;
  width: 150px;
  height: 150px;
}
.welcome {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  margin-top: -10%;
}
@media (max-width: 1400px) {
  p{
    width: 80%;
  }
}
</style>
