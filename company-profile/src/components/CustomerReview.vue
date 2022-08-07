<template>
    <div class="container-fluid py-3">
        <div class="row text-center">
            <h1>Customer Reviews</h1>
        </div>
        <div class="row">
            <div class="swiffy-slider slider-item-show2 slider-nav-sm slider-nav-page slider-item-snapstart slider-item-nogap slider-nav-round slider-nav-dark slider-indicators-dark slider-nav-animation slider-nav-animation-slideup slider-nav-autoplay" data-slider-nav-autoplay-interval="6000">
                <div class="slider-container">
                    <div class="p-5 p-xl-5 text-light" :style="{'background-color':index%2 === 0 ? '#122341' : '#233e6a'}" v-for="(review, index) in reviews" :key="index">
                        <h3 class="text-uppercase h5">{{review.consumer.displayName}}</h3>
                        <p>
                            {{review.text}}
                        </p>
                    </div>
                </div>

                <button type="button" class="slider-nav" aria-label="Go left"></button>
                <button type="button" class="slider-nav slider-nav-next" aria-label="Go left"></button>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
    data: function(){
        return{
            reviews:[]
        }
    },
    mounted(){
        const options = {
        method: 'GET',
        headers: {
            'X-RapidAPI-Key': '95ecaa2bebmsh37c9d9118042aa5p17d765jsn3612af611acd',
            'X-RapidAPI-Host': 'trustpilot4.p.rapidapi.com'
        }
        };

        fetch('https://trustpilot4.p.rapidapi.com/?domain=www.hellooma.com&page=1', options)
        .then((response) => response.json())
        .then((response) => {
            this.reviews = response.reviews
            })
        .catch(err => console.error(err));
    }
    }
</script>

<style scoped>
h1{
    font-family: 'Cormorant Garamond', serif;
}

p{
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
        font-size: 2.5rem;
    } /*1rem = 16px*/  
}

/* Large devices (desktops, 992px and up) */
@media (min-width: 992px) { 
    h1{
        font-size:4.5rem;
    } /*1rem = 16px*/
}
</style>