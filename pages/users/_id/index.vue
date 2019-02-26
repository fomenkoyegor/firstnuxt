<template>
  <div>
    <h1>
      Re is user id: {{$route.params.id}}
    </h1>
  </div>
</template>

<script>
  export  default {
    mounted() {
    },
    validate ({ params }) {
      // Must be a number
      return /^\d+$/.test(params.id)
    },
    layout:'users'
  }
</script>
