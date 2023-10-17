<script setup>
import {ref} from 'vue'

let num = ref(0)

</script>

<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark boder-bottom boder-body">
    <div class="container-fluid">
      <router-link to="/" class="navbar-brand">("NOME de algo")</router-link>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data_bs_target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item">
            <router-link to="/Login" class="nav-link" aria-current="page">Login</router-link>
          </li>
          <li class="nav-item">
            <router-link to="/Cadastre-se" class="nav-link">Cadastre-se</router-link>
          </li>

        </ul>

      </div>
    </div>
  </nav>

  <div class="main">
    <router-view></router-view>
  </div>

  <footer class="bg-dark text-light">
    <div> Unimar | ADS | {{ new Date().getFullYear() }}
    </div>
  </footer>
</template>

<style>

footer{
  position: fixed;
  bottom: 0;
  width: 100%;
  display: 100;
}
</style>