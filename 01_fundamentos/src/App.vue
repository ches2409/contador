<script>
  export default {
    data:()=>({
      contador:10,
    }),
    methods:{
      
      incrementar(){
        this.contador++
      },
      decrecer(){
        this.contador--
      },
      resetear(){
        this.contador=10
      },
    }
  }
</script>

<template>
  <div class="container">
    <img src="./assets/logo.svg" alt="Logo vue" width="125" height="125" />
    <small>
      <h1>Hola mundo desde vue.js 3</h1>
    </small>
    
    <hr />
    <h2>Contador: {{ contador }}</h2>
    <button @click="incrementar()">+1</button>
    <button @click="decrecer()"> -1</button>
    <button @click="resetear()">Reset</button>
  </div>
 
</template>

<style scoped>
  .container{
    text-align: center;
  }

  small{
    color: #666;
  }

  h1{
    font-weight:bolder;
  }

  h2{
    font-size: 1.8rem;
  }

  button{
    cursor: pointer;
    font-size: 1.5rem;
    margin: 0px 6px;
  }
</style>
