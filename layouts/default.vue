<template>
  <div>
    <nav class="navbar navbar-expand-lg navbar-dark bg-primary bg-gradient">
  <div class="container-fluid">
    <nuxt-link :to="{name:'index'}" class="navbar-brand" href="#">Laravel</nuxt-link>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <nuxt-link :to="{name:'login'}" class="nav-link" href="#">Login</nuxt-link>
        </li>
        <li class="nav-item">
          <nuxt-link :to="{name:'register'}" class="nav-link" href="#">Register</nuxt-link>
        </li>
        <li class="nav-item">
          <nuxt-link :to="{name:'register'}" class="nav-link" href="#">Dashboard</nuxt-link>
        </li>
      </ul>
    </div>
  </div>
</nav>
   <div class="container">
      <Nuxt />
   </div>
  </div>
</template>

<script>
export default {
}
</script>

<style>
@import url('https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/css/bootstrap.min.css');
</style>
