<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";

</script>

<template>
 <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">GPP System</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav">
        <li class="nav-item">
          <router-link class="nav-link active" aria-current="page" to="/">Dashboard</router-link>
        </li>
        <li class="nav-item">
          <router-link class="nav-link" to="/Login">Login</router-link>
        </li>
        <li class="nav-item">
          <router-link class="nav-link" to="/Profile">Profile</router-link>
        </li>
        <li class="nav-item">
          <router-link class="nav-link" to="/Todolist">Todolist</router-link>
        </li>
      </ul>
    </div>
  </div>
</nav>
  <router-view />
</template>

<style>
.container {
  max-width: 960px;
  margin: 0 auto;
}
h1 {
  padding-top: 40px;
  color: #039be5;
  text-align: center;
  font-size: 30px;
}
</style>