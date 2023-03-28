<template>
  <NavBar />
  <main>
    <section class="mainSection">
      <img src="./images/Vue_logo.png" alt="vue logo">
      <h1>Welcome to Vue.js</h1>
      <h3>Become a coding ninja with the fastest-growing JavaScript framework</h3>
      <button href="#"><a>Awesome!</a></button>
    </section>
    <section class="mainArticle">
      <ArticleSections 
      v-for="article in articles" 
      :key="article.id" 
      :icon="article.icon"
      :title="article.title"
      :description="article.description"
      ></ArticleSections>
    </section>
  </main>
</template>

<script>
import NavBar from './components/NavBar.vue'
import ArticleSections from './components/ArticleSection.vue'
export default {
  name: 'App',
  components: {
    NavBar,
    ArticleSections
  },
  data() {
            return {
                articles: [
                { icon: '/images/USP-3.png',
                title: 'Performant',
                description: 'Truly reactive, compiler-optimized rendering system that rarely requires manual optimization.'}, 
                { icon: '/images/USP-2.png',
                title: 'Approachable',
                description: 'Builds on top of standard HTML, CSS and JavaScript with intuitive API and world-class documentation.'}, 
                { icon:'/images/USP-3.png',
                title: 'Versatile',
                description: 'A rich, incrementally adoptable ecosystem that scales between a library and a full-featured framework.'}, 
                ]
            }
        }
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
  justify-content: center;
  text-align: center;
  letter-spacing: -0.02em;
  color: #FFFFFF;
}
.mainSection {
  display: flex;
  align-items: center;
  flex-direction: column;
}

.mainArticle {
  background-color: #39B983;
  width: 100%;
  height: 312px;
  margin-top: 65px;
  display: flex;
  justify-content: space-between;
  flex-direction: row;
}
</style>