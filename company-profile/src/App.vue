<template>
  <nav class="navbar navbar-expand-lg fixed-top text-bg-dark bg-opacity-50" >
      <div class="container">
          <a class="navbar-brand" href="#">
              <img src="./assets/img/logo.png" class="pb-1" alt="..." style="width: 100px;"/>
          </a>
          <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
              <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarSupportedContent">
              <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                  <li class="nav-item">
                      <a class="nav-link text-white active" aria-current="page" href="#">Home</a>
                  </li>
                  <li class="nav-item">
                      <a class="nav-link text-white" href="#">About</a>
                  </li>
                  <li class="nav-item">
                      <a class="nav-link text-white" href="#">Menu</a>
                  </li>
                  <li class="nav-item">
                      <a class="nav-link text-white" href="#">Blog</a>
                  </li>
                  <li class="nav-item">
                      <a class="nav-link text-white" href="#">Shop</a>
                  </li>
                  <li class="nav-item">
                      <a class="nav-link text-white" href="#">Contact</a>
                  </li>
              </ul>
              <form class="d-flex" role="search">
                  <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
                  <button class="btn btn-outline-dark" type="submit">Search</button>
              </form>
          </div>
      </div>
  </nav>
  <Banner/>
  <Menu/>
</template>

<script>
import Menu from './components/Menu.vue'
import Banner from './components/Banner.vue'

export default {
  name: 'App',
  components: {
    Menu,
    Banner
}
}
</script>
