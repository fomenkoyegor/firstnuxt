<template>
  <div>
    <h1>
      this is {{name}} page
    </h1>
    <input type="text" v-model="userId">
    <button @click="onLoadUser">Load User</button>
    <nuxt-child/>
  </div>

</template>


<script>
  export  default {
    data(){
      return {
        name:'users',
        userId:''
      }
    },
    methods:{
      onLoadUser(){
        this.$router.push(`/users/${this.userId}`)
      }
    },
    layout:'users'
  }
</script>
