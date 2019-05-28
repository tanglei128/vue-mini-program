<template>
    <div>
      <p>{{msg}}</p>
      <button @click="clickMe">点击</button>
      <i-button type="primary" @click="clickMe">这是一个按钮</i-button>
    </div>
</template>

<script>
    export default {
        name: "index",
      data(){
          return{
            msg:'hello'
          }
      },
      methods:{
        clickMe(){
            this.msg =  new Date().getTime() + '';
        }
      }
    }
</script>

<style scoped>

</style>
