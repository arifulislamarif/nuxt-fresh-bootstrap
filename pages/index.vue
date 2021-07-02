<template>
  <div class="container mt-5">
    <div class="row">
      <div class="card card-primary">
        <div class="card-header bg-primary text-light">
          Welcome to our website
        </div>
        <div class="card-body" >
          <div class="text-center">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Autem ducimus modi doloribus quae praesentium. Delectus amet voluptate necessitatibus eligendi alias?
          </div>
          <div class="text-center mt-5">
            <button class="btn btn-primary">Go to dashboard</button>
            <nuxt-link :to="{name:'register'}" class="btn btn-success">Sign Up</nuxt-link>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>
