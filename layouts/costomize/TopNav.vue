<template>
  <div>
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
      <nuxt-link class="navbar-brand" to="/"> Car Dekho </nuxt-link>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav mr-auto">
          <li class="nav-item">
            <nuxt-link class="nav-link" to="/Home"> Home </nuxt-link>
          </li>
          <li class="nav-item">
            <nuxt-link class="nav-link" to="/Dashboard"> Dashboard </nuxt-link>
          </li>
          <li class="nav-item">
            <nuxt-link class="nav-link" to="/About"> About </nuxt-link>
          </li>
        </ul>
        <form class="form-inline my-2 my-lg-0">
          <nuxt-link class="nav-link" to="/Login"> Login </nuxt-link>
          <nuxt-link class="nav-link" to="/Registeration"> Register </nuxt-link>
        </form>
      </div>
    </nav>
  </div>
</template>

<script>
export default {}
</script>