<script>
export default{
  data:() => ({
    contador:0 ,
  }),
methods:{
  aumentar(){
    this.contador += 1;
  },
  reducir(){
    this.contador -=1;
  },
  reset(){
    this.contador = 0;
  }, 
}  
}
</script>



<template>
  <div class="container">
  <img src="./assets/logo.svg" width="150" height="150">
  <h1>Hola Mundo desde vue js</h1>
  <br />
  <h2>Contador: {{ contador }}</h2>
  <button @click="aumentar">+1</button>
  <button @click="reducir">-1</button>
  <button @click="reset">Reset</button>

</div>
</template>

<style scoped>


h1{
  color:red;
}
.container{
  background: blue;
}
</style>