<template>
  <div class="row">
    <div class="col-3">
      <div class="card">
        <div class="card-header">
          Dashboard
        </div>
        <div class="card-body">
          <ul>
            <li>
              <nuxt-link :to="{name:'dashboard'}" href="">
                Dashboard
              </nuxt-link>
            </li>
            <li>
              <nuxt-link :to="{name:'dashboard-profile'}" href="">
                Profile
              </nuxt-link>
            </li>
            <li><a href="">Logout</a></li>
          </ul>
        </div>
      </div>
    </div>
    <div class="col-9">
      <nuxt-child />
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>

</style>
