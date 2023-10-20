<script setup>
import { ref } from 'vue'

const msg = ref('Hello World!')

const name = ref('')

</script>

<template>
  <div class="mainConatiner">
  <h1>{{ msg }}</h1>
  <input v-model="msg">


  <div class="SpaceBetween"></div>

    <h1>Willkommen {{name}}</h1>


    <div><p>Schreibe deinen Namen in diese Box -></p> <input v-model="name"></div>
    <div><p>Herzlich Willkomen "{{name}}", <br>
    habe ich dein Interesse geweckt? Ja? Dann versuch dich doch gleich selbst daran! <br>
    Den Link hierzu findest du auf der Website! <br>
    Welche website? -> Folge dem Link in dem QR-Code den ich bereitstelle &#128521
    </p>   
    </div>  
</div>

</template>
<style>
  .SpaceBetween{
    margin-top: 10px;
    border-bottom: 5px solid black;
  }

  body{
    height: 98vh;
    margin-left: 20vw;
    margin-right: 20vw;
    background-color: green;

  }

  .mainConatiner{
    height: 95vh;
    background-color: white;
    padding: 1rem;
  }

  h1{
    margin-left: 15%;
    margin-right: 15%;
    padding-top: 2px;
    padding-bottom: 2px;
    width: 70%;
    text-align: center;
    border: 2px solid green;
    border-radius: 20px;

    color: green;
  }

</style>