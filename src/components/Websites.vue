<template>
  <div class="container">
    <div class="wave">
      <svg
        viewBox="0 0 500 150"
        preserveAspectRatio="none"
        style="height: 100%; width: 100%"
      >
        <path
          transform="translate(0, -10)"
          d="M000,50.10 C100.00,100.33 569.20,-50.10 500.00,50.10 L500.00,100.33 L0.00,100.33 Z"
          fill="#FFF9E2"
        />
        <path
          d="M0.00,50.10 C150.00,150.33 349.20,-50.10 500.00,50.10 L500.00,150.33 L0.00,150.33 Z"
          style="fill: #f6eece"
        ></path>
      </svg>
    </div>
    <div class="text">
      <h2>websites</h2>
      <div class="parent">
        <div class="div1">
          <a href="https://github.com/AgataJacyk/bedzie5_theme"
            ><img class="project" src="/projects/bedzie5.gif"
          /></a>
        </div>
        <div class="div2">
          <a href="https://github.com/AgataJacyk/PokemonBrowser"
            ><img class="project" src="/projects/pokeAPI.gif"
          /></a>
        </div>
        <div class="div3">
          <a href="https://agatajacyk.github.io/DiceGame/dicee.html"
            ><img class="project" src="/projects/dicegame.gif"
          /></a>
        </div>
        <div class="div4">
          <a href="https://agatajacyk.github.io/MyPage/index.html"
            ><img class="project" src="/projects/mypage.gif"
          /></a>
        </div>
        <div class="div5">
          <a href="https://super-mario-pizza.netlify.app/"
            ><img class="project" src=""
          /></a>
        </div>
        <div class="div6">
          <a href="https://agatajacyk.github.io/monsterSlayer/">
            <img class="project" src="" />
          </a>
        </div>
      </div>
      <deafult-button
        ><router-link to="/Websites"
          >Click for more</router-link
        ></deafult-button
      >
    </div>
    <img class="border" src="/cream.png" />
  </div>
</template>

<script>
import DeafultButton from "../UI/buttons.vue";

export default {
  components: {
    DeafultButton,
  },
};
</script>

<style lang="scss" scoped>
a {
  font-size: calc(16px + (24 - 16) * ((100vw - 300px) / (2865 - 300)));
  line-height: 0;
  padding-top: 0.5rem;
  color: #f6eece;
}
.border {
  margin: 0 auto 0;
  width: 100%;
}
.container,
.wave {
  width: 100%;
}
.container {
  margin: 3% 0 -20%;
  z-index: 4;
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
.text {
  background-color: #f6eece;
  margin-top: -5rem;
  padding-bottom: 4rem;
}
.wave {
  height: 200px;
  margin: 0;
}
@media (max-width: 1550px) {
  .parent > div > a {
  width: 80%;
  height: 80%;
  margin: 10px 0;
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
