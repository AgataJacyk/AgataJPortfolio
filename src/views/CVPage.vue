<template>
  <div class="main_content">
    <section class="head">
      <div class="cv_header">
        <div class="parent">
          <div class="div1"><img src="/me.png" /></div>
          <div class="div2">
            <h3>Agata Jacyk</h3>
            <p>tel. 661-470-335</p>
            <p>email:agatajacyk.webdeveloper@gmail.com</p>
            <p>portfolio:agata.github.io</p>
            <p>
              if you hire me, you will gain an employee with a passion for
              creating and crossing your own borders. An ambitious person who is
              committed to his work. Together, we can create projects that go
              beyond the usual patterns, we are only limited by our imagination.
            </p>
          </div>
          <div class="div3">
            <Git />
            <LinkedIn />
          </div>
        </div>
        <img class="cream" src="/cream.png" />
      </div>
    </section>
    <section class="cv-contents">
      <h4>Education</h4>
      <p>21 / 03 / 2021</p>
      <p>
        WSB University in Gdansk - Informatics - Specialisation: Frontend
        Developer
      </p>
      <br />
      <p>1 / 09 / 2013 - 22 / 05 / 2016</p>
      <p>IV Secondary School of Tadeusz Kościuszko in Toruń</p>
      <hr />
      <p>15 / 08 / 2020 - 20 / 03 / 2021</p>
      <p>Software Development Academy - Java from scratch</p>
      <hr />
      <h4>Skills</h4>
      <table>
        <tbody>
          <tr>
            <td>
              <ul>
                <li>HTML 5</li>
                <li>CSS 3</li>
                <li>Java Script(ES6)</li>
                <li>Web Design</li>
                <li>GitHub</li>
              </ul>
            </td>
            <td>
              <ul>
                <li>React.js</li>
                <li>Node.js</li>
                <li>Angular</li>
                <li>Vue.js</li>
                <li>SQL</li>
              </ul>
            </td>
            <td>
              <ul>
                <li>Design Patterns</li>
                <li>Figma</li>
                <li>Gimp</li>
                <li>Procreate</li>
                <li>Canva</li>
              </ul>
            </td>
         </tr>
        </tbody>
      </table>
      <hr />
      <ul>
        <li>good communication</li>
        <li>teamplayer</li>
        <li>organisation</li>
        <li>driving licence</li>
        <li>i'm really good at googling and searching informations</li>
      </ul>
      <hr />
      <h4>Languages</h4>
      <ul>
        <li>Polish (native)</li>
        <li>English (B2)</li>
        <li>Spanish (A1)</li>
      </ul>

      <hr />
      <h4>Hobbies</h4>
      <ul>
        <li>programming and web design</li>
        <li>drawing, digital art</li>
        <li>asian culture, kpop</li>
        <li>tattoo artist</li>
      </ul>
      <hr />
      <h4>Other</h4>
      <p>1 / 13 / 2022 - 1 / 9 / 2023</p>
      <p>Scholarship</p>
    </section>
  </div>
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
h3 {
  margin: 10% 0 0 0;
  font-size: calc(46px + (56 - 46) * ((100vw - 300px) / (2865 - 300)));
}
h3,
h4 {
  padding: 0;
}
h4 {
  font-size: calc(30px + (46 - 30) * ((100vw - 300px) / (2865 - 300)));
  margin: 0;
}
img {
  width: 90%;
  margin: 5% 0 0 10%;
}
ul {
  width: 100%;
}
li {
  display: list-item;
  text-align: left;
  list-style-type: disc;
}

p {
  color: #fb7baa;
  padding: 0 20px;
  text-shadow: none;
  margin: 0;
  margin-bottom: 1rem;
  line-height: 2rem;
  width: 100%;
}
table {
  width: 100%;
}
td {
  width: 25%;
}
.cv-contents {
  margin: 20% 5%;
  width: 90%;
  padding-bottom: 50px;
}
.cv-contents p,
li {
  color: #000000;
}
.cream {
  margin: 0;
  width: 100%;
}
.cv_header {
  width: 100%;
  height: 550px;
  border-radius: 187px 0px;
}
.main_content {
  background-color: #beeff8;
  box-shadow: 6px 6px 0px #e2fafe;
  border-radius: 187px 0px;
  height: auto;
  width: 80%;
  margin: 3% 10%;
}
.parent {
  background-color: #f6eece;
  display: grid;
  grid-template-columns: 2fr 3fr 1fr;
  grid-template-rows: 1fr;
  grid-column-gap: 0;
  width: 100%;
  border-radius: 187px 0 0 0;
  margin: 0;
}
.div1 {
  grid-area: 1 / 1 / 2 / 2;
}
.div2 {
  grid-area: 1 / 2 / 2 / 3;
}
.div3 {
  grid-area: 1 / 3 / 2 / 4;
  padding-top: 30%;
  width: 80%;
}
.div3 li {
  list-style-type: none;
}
@media (max-width: 1400px) {
  img {
    width: 50%;
    margin: 10% 0 0;
  }
  .cv-contents {
    margin: 60% 3px 10%;
  }
  .parent {
    grid-template-columns: 3fr 1fr;
  }
  .div1 {
    grid-area: 1 / 1 / 2 / 3;
    display: flex;
    justify-content: center;
  }
  .div2 {
    grid-area: 2 / 1 / 3 / 2;
    padding-left: 30px;
  }
  .div3 {
    grid-area: 2 / 2 / 3 / 3;
    padding-top: 100%;
  }

}
@media (max-width: 925px) {
  .cv-contents {
    margin: 60% 3%;
  }
  p {
    padding: 0 10px;
  }
  li, p {
    line-height: 1rem;
  }
}
@media (max-width: 438px) {
  .div3 {
    margin-left: -80px;
  }
}
</style>
