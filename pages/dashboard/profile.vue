<template>
     <div class="card">
        <div class="card-header">
          My Profile
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
              Update Profile
            </button>
          </form>
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
