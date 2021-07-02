<template>
  <div class="row justify-content-center">
    <div class="col-6">
      <div class="card">
        <div class="card-header">
          Login Page
        </div>
        <div class="card-body">
          <form @submit.prevent="userLogin">
            <div class="mb-3">
              <label class="form-label">Email address</label>
              <input
                v-model="login.email"
                type="email"
                class="form-control"
              >
            </div>
            <div class="mb-3">
              <label class="form-label">Password</label>
              <input
                v-model="login.password"
                type="password"
                class="form-control"
              >
            </div>
            <button type="submit" class="btn btn-primary">
              Submit
            </button><br>
            <span>Don't have an account?</span>
            <nuxt-link :to="{name:'register'}" href="#">
              Signup
            </nuxt-link>Now
          </form>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      login: {
        email: 'developer@mail.com',
        password: 'password'

      }
    }
  },
  methods: {
    async userLogin () {
      try {
        const response = await this.$auth.loginWith('local', { data: this.login })
        console.log(response)
      } catch (err) {
        console.log(err)
      }
    }
  }
}
</script>

<style>

</style>
