<template>
  <CommonContainer>
    <div class="mess">
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
    </div>
  </CommonContainer>
</template>
<script>
import CommonContainer from "../UI/CommonContainer.vue";

export default {
  components: {
    CommonContainer,
  },
};
</script>

<style scoped>
a {
  width: 80%;
  height: 80%;
  margin: 20px;
}

a:hover {
  background-color: #fb7baa;
  border-radius: 60px;
  padding: 0;
  margin: 20px;
}
@media (max-width: 1400px) {
  .container {
    padding-bottom: 30%;
    margin-bottom: -15%;
  }
  .parent > div > a {
  width: 80%;
  height: 80%;
  margin: 10px 0;
  }
  .parent { 
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: repeat(4, 1fr);
    margin: 0;
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
