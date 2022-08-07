<template>
    <div class="container text-center">
        <div class="row mt-3">
            <h1>Our Branches</h1>
        </div>
        <div class="row">
            <div class="col-12 col-md-6 col-lg-4 px-0 mx-auto my-3 shadow-lg card border border-0" style="width: 18rem;">
                <img src="../assets/img/city_1.jpg" alt="...">
                <div class="card-body p-0 text-start">
                    <h3 class="card-title d-inline-flex mt-3 px-3 py-1 col-6 col-md-8 rounded-end text-light">New York</h3>
                    <p class="card-text p-3 text-center text-light m-3 fw-light fs-6">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Sit aperiam sint deserunt repellendus consequatur dolorem doloribus a laboriosam rem, sequi ut molestiae incidunt ea odit ipsam pariatur. Fugiat, repellat quos! </p>
                </div>
            </div>
            <div class="col-12 col-md-6 col-lg-4 px-0 mx-auto my-3 shadow-lg card border border-0" style="width: 18rem;">
                <img src="../assets/img/city_2.jpg" alt="...">
                <div class="card-body p-0 text-start">
                    <h3 class="card-title d-inline-flex mt-3 px-3 py-1 col-6 col-md-8 rounded-end text-light">Texas</h3>
                    <p class="card-text p-3 text-center text-light m-3 fw-light fs-6">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Sit aperiam sint deserunt repellendus consequatur dolorem doloribus a laboriosam rem, sequi ut molestiae incidunt ea odit ipsam pariatur. Fugiat, repellat quos! </p>
                </div>
            </div>
            <div class="col-12 col-md-6 col-lg-4 px-0 mx-auto my-3 shadow-lg card border border-0" style="width: 18rem;">
                <img src="../assets/img/city_3.jpg" alt="...">
                <div class="card-body p-0 text-start">
                    <h3 class="card-title d-inline-flex mt-3 px-3 py-1 col-6 col-md-8 rounded-end text-light">New Jersey</h3>
                    <p class="card-text p-3 text-center text-light m-3 fw-light fs-6">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Sit aperiam sint deserunt repellendus consequatur dolorem doloribus a laboriosam rem, sequi ut molestiae incidunt ea odit ipsam pariatur. Fugiat, repellat quos! </p>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
h1{
    font-family: 'Cormorant Garamond', serif;
}

h3{
    font-family: 'PT Sans', sans-serif;
}

.open{
    background-color: #122341;
}

.card-body{
    background-color: #233e6a;
}

.card-title{
    background-color: #ff4a00;
}

.card-text{
    background-color: #122341;
}

/* Small devices (landscape phones, 544px and up) */
@media (max-width: 544px) {  
    h1{
        font-size: 2.5rem;
    } /*1rem = 16px*/ 

    h3{
        font-size: 1.5rem;
    }
}

/* Medium devices (tablets, 768px and up) The navbar toggle appears at this breakpoint */
@media (min-width: 544px) {  
    h1{
        font-size: 3.5rem;
    } /*1rem = 16px*/ 
    h3{
        font-size: 1.5rem;
    }
}

/* Large devices (desktops, 992px and up) */
@media (min-width: 992px) { 
    h1{
        font-size:4.5rem;
    } /*1rem = 16px*/
    h3{
        font-size: 2rem;
    }
}
</style>