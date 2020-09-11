<template>
  <nav class="navbar navbar-expand-lg navbar-light">
    <router-link class="navbar-brand" to="/"
      ><img id="logo" src="../assets/logo_bg.png" alt=""
    /></router-link>
    <button
      class="navbar-toggler"
      type="button"
      data-toggle="collapse"
      data-target="#navbarSupportedContent"
      aria-controls="navbarSupportedContent"
      aria-expanded="false"
      aria-label="Toggle navigation"
    >
      <span class="navbar-toggler-icon"></span>
    </button>

    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav ml-auto">
        <li class="nav-item active">
          <router-link class="nav-link" to="/">
            Home
          </router-link>
        </li>
        <li class="nav-item active">
          <router-link class="nav-link" to="#">Profile</router-link>
        </li>
        <li class="nav-item active">
          <router-link class="nav-link" to="#">Skills</router-link>
        </li>
        <li class="nav-item active">
          <router-link class="nav-link" to="#">Articles</router-link>
        </li>
        <li class="nav-item active">
          <router-link class="nav-link" to="#">Contact me</router-link>
        </li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  name: "Navbar",
};
</script>

<style>
.navbar {
  padding-left: 1rem;
  padding-right: 1rem;
  padding-top: 2rem;
}

.nav-item {
  text-align: right;
}

.navbar-toggler-icon {
  font-size: 0.8rem;
}

.navbar-light .navbar-nav .active > .nav-link,
.navbar-light .navbar-nav .nav-link.active,
.navbar-light .navbar-nav .nav-link.show,
.navbar-light .navbar-nav .show > .nav-link {
  font-weight: 1000;
  padding: 0.8rem 0.8rem;
  font-family: "Comfortaa";
}

#logo {
  height: 2rem;
}

.navbar-collapse {
  background: none;
  padding: none;
}

@media screen and (min-width: 991px) {
  .navbar {
    padding-left: 5rem;
    padding-right: 5rem;
    padding-top: 2rem;
  }
}
</style>
