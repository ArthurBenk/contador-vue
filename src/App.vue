<script setup>
import {ref} from 'vue'

const contador = ref(0)

function incrementar(){
  contador.value++
}
function tirar(){

  if (contador.value > 0) {
    contador.value--
  }

}
function resetar(){
  contador.value=0
}
</script>

<template>
  <h1>meu contador legalzão em vue</h1>
  <p>valor do contador: {{contador}}</p>
  <button v-on:click="incrementar">+</button>
  <button v-on:click="tirar">-</button>
  <button v-on:click="resetar">reset</button>
</template>

<style scoped>
 template{
  background-color: grey;
 }
</style>
 