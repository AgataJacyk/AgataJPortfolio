<template>
  <CommonContainer>
    <div class="mess">
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
    </div>
  </CommonContainer>

  <CommonContainer>
    <div class="mess">
      <h2>drawings</h2>
      <div class="parent">
        <div class="div1">
          <a href="/projects/coven.png"
            ><img class="project" src="/projects/coven.png"
          /></a>
        </div>
        <div class="div2">
          <a href="/projects/1.jpg"
            ><img class="project" src="/projects/1.jpg"
          /></a>
        </div>
        <div class="div3">
          <a href="/projects/2.jpg"
            ><img class="project" src="/projects/2.jpg"
          /></a>
        </div>
        <div class="div4">
          <a href="/projects/5.jpg"
            ><img class="project" src="/projects/5.jpg"
          /></a>
        </div>
        <div class="div5">
          <a href="/projects/gin.png"
            ><img class="project" src="/projects/gin.png"
          /></a>
        </div>
        <div class="div6">
          <a href="/projects/brerep.png"
            ><img class="project" src="/projects/brerep.png"
          /></a>
        </div>
        <div class="div7">
          <a href="/projects/prince.jpg"
            ><img class="project" src="/projects/prince.jpg"
          /></a>
        </div>
        <div class="div8">
          <a href="/projects/easterbunny.png"
            ><img class="project" src="/projects/easterbunny.png"
          /></a>
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
<style lang="scss" scoped>
a {
  width: 80%;
  height: 80%;
  margin: 20px;
  &:hover {
    background-color: #fb7baa;
    border-radius: 60px;
    padding: 0;
    margin: 20px;
  }
}
@media (max-width: 1400px) {
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
