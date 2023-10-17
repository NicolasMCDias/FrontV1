<script setup>
import {ref} from 'vue'

let num = ref(0)

</script>

<template>
 <div class="card" style="width: 25rem;display: grid;place-items: center;">
  <div class="card-header" style="border: 100%;">
    <h4>Login:</h4>
  </div>
  <div class="card-body">
    <h6 class="card-title">CPF</h6>
    <input class="form-control" type="text" placeholder="Inserir CPF" aria-label="default input example">
    <!--Area da senha-->
    <br>
    <label for="inputPassword5" class="form-label">Senha:</label>
    <input type="password" id="inputPassword5" class="form-control" aria-describedby="passwordHelpBlock" placeholder="Inserir Senha">
  </div>
  <div>
      <router-link href="#" class="btn btn-primary"  type="password" style="position:static;left:50%;transform: translate(-50%,-50%);">Entrar</router-link >
  </div> 
 </div>
</template>
