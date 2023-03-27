<template>
  <NavBar />
  <main>
    <section class="mainSection">
      <img src="" alt="vue logo">
      <h1>Welcome to Vue.js</h1>
      <h3>Become a coding ninja with the fastest-growing JavaScript framework</h3>
      <button><a>Awesome!</a></button>
    </section>
    <section class="mainArticle">
      <ArticleSections>
        
      </ArticleSections>
    </section>
  </main>
</template>

<script>
import NavBar from './components/NavBar.vue'
import ArticleSections from './components/Article.vue'
export default {
  name: 'App',
}

</script>

<style scoped>
h1 {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 800;
  font-size: 50px;
  line-height: 95px;
  letter-spacing: -0.02em;
  color: #2B2F30;

}

h3 {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 800;
  font-size: 14px;
  line-height: 20px;
  color: #2B2F30;

}

img {
 margin-top: 28px;
 width: 129px;
 height: 129px
}

button {
  position: absolute;
  width: 121px;
  height: 31px;
  margin-top: 22px;
  background: #34495E;
  border-radius: 13px;
}

button a{
  font-family: 'Inter';
  font-style: normal;
  font-weight: 800;
  font-size: 14px;
  line-height: 20px;
  display: flex;
  align-items: center;
  text-align: center;
  letter-spacing: -0.02em;
  color: #FFFFFF;
}
.mainSection {
  display: flex;
  justify-content: center;
  flex-direction: column;
}

.mainArticle {
  background-color: #39B983;
  position: absolute;
  width: 600px;
  height: 312px;
  margin-top: 65px
}
</style>