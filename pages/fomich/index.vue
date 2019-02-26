<template>
  <div>
    <app-logo/>
    <ul>
      <li v-for="fruit in fruits" :key="fruit.id">
        <h3>{{fruit.name}}</h3>
        <a >re</a>
      </li>
    </ul>
  </div>
</template>

<script>
  import AppLogo from '~/components/AppLogo.vue'
  export default {
    components: {
      AppLogo
    },
    name: "index",
    data() {
      return {
        fruits: [
          {id: 1, name: "banana"},
          {id: 2, name: "ananas"},
          {id: 3, name: "cocos"},
        ]
      };
    }
  }
</script>

<style scoped>

</style>
