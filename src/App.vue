<template>
  <div id="app">
    <blog-post
      v-for="post in posts"
      v-bind:key="post.id"
      v-bind:title="post.title">
    </blog-post>
    <button-counter></button-counter>
  </div>
</template>

<script>
import BlogPost from './components/BlogPost.vue'
import ButtonCounter from './components/ButtonCounter.vue'

export default {
  name: 'app',
  components: {
        BlogPost,

        ButtonCounter
  },
  data: function() {
    return {
      posts: [
        { id: 1, title: 'My journey with Vue' },
        { id: 2, title: 'Blogging with Vue' },
        { id: 3, title: 'Why Vue is so fun' }
      ]
    }
  }

  
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
