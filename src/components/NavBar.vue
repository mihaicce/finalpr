<template>
<header>
  <!-- Navbar -->
  <nav class="navbar navbar-expand-lg navbar-light fixed-top mask-custom shadow-0">
    <div class="container m-0">
      <router-link to="/"><a class="navbar-brand" href="#!"><img src="../assets/logoApdent.png" alt="Logo"></a></router-link>
      <button class="navbar-toggler" type="button" data-mdb-toggle="collapse"
        data-mdb-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false"
        aria-label="Toggle navigation">
        <i class="fas fa-bars"></i>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto">
          <li class="nav-item">
            <router-link class="nav-link" to="/">Home</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/about">Despre Noi</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/about">Servicii</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/about">Preturi</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/about">Echipa</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/about">Contact</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/Programare"><button class="btn btn-light programare">Programeaza-te</button></router-link>
          </li>
        </ul>
      </div>
    </div>
  </nav>
  <!-- Navbar -->

  <!--Section: Design Block-->

  <!--Section: Design Block-->
</header>
</template>

<script>
export default {
  name: 'NavBar',
  // props: {
  //   msg: String
  // }
}
</script>

<style>
/* .bg-custom {
    background-color: #96C40A;
  } */

  /* Color of the links BEFORE scroll */
/* .navbar-scroll .nav-link,
.navbar-scroll .navbar-toggler-icon,
.navbar-scroll .navbar-brand {
  color: #fff;
} */

/* Color of the links AFTER scroll */
/* .navbar-scrolled .nav-link,
.navbar-scrolled .navbar-toggler-icon,
.navbar-scrolled .navbar-brand {
  color: #fff;
} */

/* Color of the navbar AFTER scroll */
/* .navbar-scroll,
.navbar-scrolled {
  background-color: #cbbcb1;
} */

.mask-custom {
  backdrop-filter: blur(5px);
  background-color: rgba(150, 196, 10, .48);
}

.navbar-brand {
  font-size: 1.75rem;
  letter-spacing: 3px;
}

.navbar-collapse {
  flex-grow: 0 !important;
}

.navbar-expand-lg {
  justify-content: space-evenly !important;
}

</style>