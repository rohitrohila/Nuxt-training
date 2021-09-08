<template>
    <div>
        <nav class="navbar navbar-expand-lg navbar-light bg-light">
            <nuxt-link class="navbar-brand" to="/">
             Car Dekho
            </nuxt-link>
  <div class="collapse navbar-collapse" id="navbarSupportedContent">
    <ul class="navbar-nav mr-auto">
      <li class="nav-item">
          <nuxt-link class="nav-link" to="/About">
             About
            </nuxt-link>
      </li>
            <li class="nav-item">
          <nuxt-link class="nav-link" to="/Login">
             Login
            </nuxt-link>
      </li>

      <li class="nav-item">
          <nuxt-link class="nav-link" to="/Registeration">
             Register
            </nuxt-link>
      </li>


    </ul>
    <form class="form-inline my-2 my-lg-0">
      <input class="form-control mr-sm-2" type="search" placeholder="Search" aria-label="Search">
      <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Search</button>
    </form>
  </div>
</nav>
    </div>
</template>

<script>
export default {
        
    }
</script>