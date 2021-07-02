<template>
    <div class="row justify-content-center">
    <div class="col-6">
      <div class="card">
        <div class="card-header">
          Create an account
        </div>
        <div class="card-body">
          <form>
            <div class="mb-3">
              <label class="form-label">Name</label>
              <input type="test" class="form-control">
            </div>
            <div class="mb-3">
              <label class="form-label">Email address</label>
              <input type="email" class="form-control">
            </div>
            <div class="mb-3">
              <label class="form-label">Password</label>
              <input  type="password" class="form-control">
            </div>
            <button type="submit" class="btn btn-primary">
              Submit
            </button><br>
             <span>Already have an account?</span>
            <nuxt-link :to="{name:'login'}" href="#">
              Signin
            </nuxt-link>Now
          </form>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>

</style>
