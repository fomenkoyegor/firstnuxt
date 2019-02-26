<template>
  <section>
   <!--<Header/>-->

    <div>
      <h1>Posts</h1>
    </div>
    <div class="posts">
      <Post v-for="post in posts"
            :key="post.id"
            :post="post"
      />
    </div>


  </section>

</template>

<script>
import Header from "../components/Header";
import Post from "../components/Post";

export default {
  components: {
    Post,
    Header
  },
  data(){
    return {
      posts:[
        {id:1,title:"re1",img:'https://images.unsplash.com/photo-1551122560-c4bed8cdcc15?ixlib=rb-1.2.1&q=80&fm=jpg&crop=entropy&cs=tinysrgb&w=1080&fit=max&ixid=eyJhcHBfaWQiOjE5Mzk5fQ'},
        {id:2,title:"re2",img:'https://images.unsplash.com/photo-1551092868-0b77c6db2537?ixlib=rb-1.2.1&q=80&fm=jpg&crop=entropy&cs=tinysrgb&w=1080&fit=max&ixid=eyJhcHBfaWQiOjE5Mzk5fQ'},
        {id:3,title:"re3",img:'https://images.unsplash.com/photo-1551103124-78b59627166e?ixlib=rb-1.2.1&q=80&fm=jpg&crop=entropy&cs=tinysrgb&w=1080&fit=max&ixid=eyJhcHBfaWQiOjE5Mzk5fQ'},
        {id:4,title:'qw',img:'https://images.unsplash.com/photo-1542834281-979df8f0a97b?ixlib=rb-1.2.1&q=80&fm=jpg&crop=entropy&cs=tinysrgb&w=1080&fit=max&ixid=eyJhcHBfaWQiOjE5Mzk5fQ'}
      ]
    }
  }
}
</script>

<style scoped>
  .posts{
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
  }


</style>

