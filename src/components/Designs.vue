<template>
  <div class="container">
      <h2>designs</h2>
      <div class="parent">
        <div class="div1">
          <a href="https://agatajacyk.github.io/MyPage/index.html"
            ><img class="project" src="/projects/savetheocean.gif"
          /></a>
        </div>
        <div class="div2">
          <a href="https://agatajacyk.github.io/MyPage/index.html"
            ><img class="project" src="/projects/mountain.gif"
          /></a>
        </div>
        <div class="div3">
          <a href="https://agatajacyk.github.io/MyPage/index.html"
            ><img class="project" src="/projects/coffee.gif"
          /></a>
        </div>
        <div class="div4">
          <a href="https://agatajacyk.github.io/MyPage/index.html"
            ><img class="project" src="/projects/icecream.gif"
          /></a>
        </div>
        <div class="div5">
          <a href="https://agatajacyk.github.io/MyPage/index.html"
            ><img class="project" src="/projects/AnimalCare.gif"
          /></a>
        </div>
        </div>
      <deafult-button><router-link to="/Designs">Click for more</router-link></deafult-button>
    </div>
</template>

<script>
import DeafultButton from '../UI/buttons.vue'

export default {
    components: {
    DeafultButton
    }
    }
</script>

<style lang="scss" scoped>
a {
  font-size: calc(16px + (24 - 16) * ((100vw - 300px) / (2865 - 300)));
  line-height: 0;
  padding-top: 8px;
  color: #F6EECE;
}
.container {
  width: 100%;
  z-index: 2;
  background-color: #fdcce0;
  padding: 15% 0 15% 0;
  margin: 3% 0 -5%;
  background-image: url(/sprinkles.png);
  background-repeat: no-repeat;
  background-size: 30%;
  background-position: right top;
}
.parent > div > a {
  width: 80%;
  height: 80%;
  margin: 0 0 40px 0 ;
  padding: 0;

  &:hover {
    background-color: #fb7baa;
    border-radius: 60px;
    padding: 0;
    margin: 0;
  }
}

@media (max-width: 1550px) {
  .container {
    padding-bottom: 30%;
    margin-bottom: -15%;
  }
  .parent > div > a {
  width: 80%;
  height: 80%;
  margin: 10px  0;
  }
  .parent { 
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: repeat(4, 1fr);
  }
  
  .div1 {
    grid-area: 1 / 1 / 2 / 2;
  }
  .div2 {
    grid-area: 1 / 2 / 2 / 3;
  }
  .div3 {
    grid-area: 2 / 1 / 3 / 2;
  }
  .div4 {
    grid-area: 2 / 2 / 3 / 3;
  }
  .div5 {
    grid-area: 3 / 1 / 4 / 2;
  }
  .div6 {
    grid-area: 3 / 2 / 4 / 3;
  }
  .div7 {
    grid-area: 4 / 1 / 5 / 2;
  }
  .div8 {
    grid-area: 4 / 2 / 5 / 3;
  }
}
</style>
