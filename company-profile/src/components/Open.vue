<template>
<div class="open">
    <div class="container text-center py-4">
        <div class="row text-light">
            <h1>We Are Open</h1>
        </div>
        <div class="row d-grid gap-5 my-4 open">
            <div class="schedule col-9 col-md-7 col-lg-4 text-light p-3 gap-3 mx-auto shadow-lg">
                <h3>Monday - Friday</h3>
                <h3>8:00 am - 11:30 pm</h3>
            </div>
            <div class="schedule col-9 col-md-7 col-lg-4 text-light p-3 gap-3 mx-auto shadow-lg">
                <h3>Saturday and Sunday</h3>
                <h3>9:00 am - 10:30 pm</h3>
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

.schedule{
    background-color: #233e6a;
}


/* Small devices (landscape phones, 544px and up) */
@media (max-width: 544px) {  
    h1{
        font-size: 2.5rem;
    } /*1rem = 16px*/ 

    h3{
        font-size: 1rem;
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