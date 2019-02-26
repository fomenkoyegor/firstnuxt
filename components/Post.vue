<template>
  <nuxt-link :to="'/posts/'+post.id" class="post">
    <div class="bg" :style="{ backgroundImage: 'url('+post.img+')'}"></div>
    <p>{{post.title}}</p>
  </nuxt-link>
</template>

<script>
  export default {
    name: "Post",
    props: {
      post: {
        type: Object,
        required: true
      }
    }
  }
</script>

<style scoped>
  .post {
    border: 1px solid;
    width: 30%;
    height: 30vh;
    margin: 10px 0;
  }

  .post .bg {
    background-position: center !important;
    background-size: cover !important;
    background-repeat: no-repeat !important;
    width: 100%;
    height: 100%;
  }

  @media (max-width: 786px) {
    .post {
      width: 45%;
    }
  }

  @media (max-width: 375px) {
    .post {
      width: 100%;
    }
  }
</style>
