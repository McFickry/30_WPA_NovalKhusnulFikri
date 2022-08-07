<template>
    <div class="section-1 pt-5 pb-3">
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <h1 class="fst-italic mt-3 mt-lg-5">Coffee</h1>
                    <h3 class="mt-4 text-capitalize">everything you love about coffee</h3>
                    <p class="col-8 col-md-6 col-lg-5 mb-3 mb-lg-5">Lorem ipsum dolor sit amet consectetur adipisicing elit. Architecto, vero voluptates magnam quis, assumenda quasi minus corporis quisquam harum fugiat facere ipsa. Id fuga eligendi totam eveniet ullam, dolore quaerat.</p>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.section-1{
    background-image: url("../assets/img/banner.jpg");
    background-repeat: no-repeat;
    background-size: cover;
}

h1{
    font-family: 'Cormorant Garamond', serif;
}

h3{
    color: #ff4a00;
}


/* Small devices (landscape phones, 544px and up) */
@media (max-width: 544px) {  
    /* .section-1{
    background-size: auto;
    } */
}

/* Medium devices (tablets, 768px and up) The navbar toggle appears at this breakpoint */
@media (max-width: 992px) {  
    h1{
        font-size: 5rem;
    } /*1rem = 16px*/

    h3{
    font-size: 0.99rem;
    }

    p{
        font-size: 0.5rem;
    }    
}

/* Large devices (desktops, 992px and up) */
@media (min-width: 992px) { 
    h1{
        font-size:7.5rem;
    } /*1rem = 16px*/

    h3{
        font-size: 2rem;
    }

    p{
        font-size: 0.9rem;
    }
}
</style>