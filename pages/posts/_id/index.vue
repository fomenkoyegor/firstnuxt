<template>
  <div>
    <h1>Post by id : {{$route.params.id}}</h1>
  </div>
</template>

<script>
  export default {
    name: "index.vue",
    validate({params}) {
      // Must be a number
      return /^\d+$/.test(params.id)
    },
  }

</script>

<style scoped>

</style>
