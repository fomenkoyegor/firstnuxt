<template>
    <header>
      <ul class="nav-items">
        <li>
          <nuxt-link to="/">home</nuxt-link>
        </li>
        <li>
          <nuxt-link to="/users">users</nuxt-link>
        </li>
      </ul>
    </header>
</template>

<script>
    export default {
        name: "Header"
    }
</script>

<style scoped>
  header{
    background: #47494e;
    width: 100%;
    height: 60px;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  header .nav-items{
    display: flex;
    justify-content: space-around;
    align-items: center;
    width: 80%;
  }

  header a{
    color: wheat;
    transition: 1s;
  }

  header a.active,header a:hover{
    color: red;
  }
</style>
