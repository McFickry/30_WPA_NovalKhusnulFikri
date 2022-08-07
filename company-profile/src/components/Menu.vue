<template>
    <div class="section-2 py-3">
        <div class="container">
            <div class="row">
                <h1>Our Product</h1>
            </div>
            <div class="row">
                <div class="swiffy-slider slider-item-show6 slider-item-reveal slider-nav-round slider-nav-outside-expand slider-nav-noloop">
                    <ul class="slider-container py-4" id="slider2">
                        <li v-for="(menu, index) in menus" :key="index">
                            <div class="card shadow h-100">
                                <div class="ratio ratio-1x1">
                                    <img :src="'/galery/'+menu.img" class="card-img-top" loading="lazy" alt="...">
                                </div>
                                <div class="card-body d-flex flex-column flex-md-row">
                                    <div class="flex-grow-1">
                                        <strong>{{menu.nama}}</strong>
                                        <p class="card-text desc">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                                    </div>
                                    <div class="px-md-2">${{menu.harga}}</div>
                                </div>
                            </div>
                        </li>
                    </ul>
                    <button type="button" class="slider-nav" aria-label="Go to previous"></button>
                    <button type="button" class="slider-nav slider-nav-next" aria-label="Go to next"></button>
                </div>
            </div>
        </div>
    </div>
</template>
<script>

export default {
    data: function(){
        return{
            menus:[]
        }
    },
    mounted(){
        fetch("/menu.json")
        .then(res => res.json())
        .then(res => {
            this.menus = res
        })
    }
}

</script>


<style scoped>
.section-2{
    background-color: #122341;
}

h1{
    color: white;
    text-align: center;
    font-family: 'Cormorant Garamond', serif;
}

.desc{
    font-family: 'PT Sans', sans-serif;
}
/* Small devices (landscape phones, 544px and up) */
@media (max-width: 544px) {  
    h1{
        font-size: 2.5rem;
    } /*1rem = 16px*/  
}

/* Medium devices (tablets, 768px and up) The navbar toggle appears at this breakpoint */
@media (min-width: 544px) {  
    h1{
        font-size: 3.5rem;
    } /*1rem = 16px*/  
}

/* Large devices (desktops, 992px and up) */
@media (min-width: 992px) { 
    h1{
        font-size:4.5rem;
    } /*1rem = 16px*/
}
</style>