<template>
    <nav id="navbar-example2" class="navbar navbar-dark navbar-expand-lg fixed-top bg-dark" >
        <div class="container">
            <a class="navbar-brand d-flex" href="#">
                <img src="./assets/img/logo.png" class="pb-1" alt="..." style="width: 100px;"/>
            </a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon text-white"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                    <li class="nav-item">
                        <a class="nav-link active" aria-current="page" href="#scrollspyHeading1">Home</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#scrollspyHeading2">Product</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#scrollspyHeading3">About</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#scrollspyHeading4">Reviews</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#scrollspyHeading5">Shop</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#scrollspyHeading6">Contact</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
    <div class="content"  data-bs-spy="scroll" data-bs-target="#navbar-example2" data-bs-smooth-scroll="true">
        <Banner id="scrollspyHeading1"/>
        <Menu id="scrollspyHeading2"/>
        <About id="scrollspyHeading3"/>
        <Open/>
        <Customer id="scrollspyHeading4"/>
        <Branch id="scrollspyHeading5"/>
        <Contact id="scrollspyHeading6"/>
    </div>
    <div class="footer text-light text-center border-top border-light">
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <p class="m-0 py-1">CoffeCup © 2022 powered by Personal. all right reserved.</p>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import Menu from './components/Menu.vue'
import Banner from './components/Banner.vue'
import About from './components/AboutUs.vue'
import Customer from './components/CustomerReview.vue'
import Open from './components/Open.vue'
import Branch from './components/Branch.vue'
import Contact from './components/Contact.vue'

export default {
  name: 'App',
  components: {
    Menu,
    Banner,
    About,
    Customer,
    Open,
    Branch,
    Contact
}
}
</script>

<style scoped>
#navbar-example2{
    background-color: #122341 !important;
}

.footer{
    background-color: #122341 !important;
}

.nav-link{
    padding-left: 25px !important;
    padding-right: 25px !important;
}
</style>