<script >

import { Swiper, SwiperSlide } from 'swiper/vue';

import 'swiper/swiper-bundle.min.css';


import { Autoplay, Pagination, Navigation } from 'swiper';

export default {
    components: {
        Swiper,
        SwiperSlide,
    },
    setup() {
        return {
            modules: [Autoplay, Pagination, Navigation],
        };
    },
};
</script>

<template>
    <div>


        <div class="container mx-auto pt-3">
            <div class="flex flex-wrap text-center">
                <div class="w-full sm:w-1/3"></div>
                <div class="w-full sm:w-1/3">
                    <h1 class="title">
                        Latest<br />
                        Updates
                    </h1>
                </div>
                <div class="w-full sm:w-1/3"></div>
            </div>
        </div>
        <div class="container mx-auto">
            <swiper 
            :a11y="true"
            :autoplay="{ delay: 5000, disableOnInteraction: false }"
            :loop="true"
            :modules="modules"
            :slides-per-view="3"
            :space-between="20"
        >
            <swiper-slide class=" bg-green-100">
                <div class="w-full">
                    <div class="container-post">
                        <a href="$">
                            <div class="container-img-post">
                                <figure>
                                    <img src="https://handmade.company/goat/img/home/blog/blog1.webp" />
                                </figure>
                                <div class="pt-8 w-auto">
                                    <h3 class="mt-0.5 text-start container-title-post">
                                        How to position your furniture for positivity
                                    </h3>
                                    <p class="mt-2 line-clamp-3 text-start container-text-post">
                                        Lorem ipsum dolor sit amet, consectetur adipisicing elit.
                                        Recusandae dolores.
                                    </p>
                                </div>
                            </div>
                        </a>
                    </div>
                </div>
            </swiper-slide>
            <swiper-slide class="bg-red-100">
                <div class="w-full">
                    <div class="container-post">
                        <a href="$">
                            <div class="container-img-post">
                                <figure>
                                    <img src="https://handmade.company/goat/img/home/blog/blog3.webp" />
                                </figure>
                                <div class="pt-8 w-auto">
                                    <h3 class="mt-0.5 text-start container-title-post">
                                        How to position your furniture for positivity
                                    </h3>
                                    <p class="mt-2 line-clamp-3 text-start container-text-post">
                                        Lorem ipsum dolor sit amet, consectetur adipisicing elit.
                                        Recusandae dolores.
                                    </p>
                                </div>
                            </div>
                        </a>
                    </div>
                </div>
            </swiper-slide>
            <swiper-slide class="bg-red-100">
                <div class="w-full">
                    <div class="container-post">
                        <a href="$">
                            <div class="container-img-post">
                                <figure>
                                    <img src="https://handmade.company/goat/img/home/blog/blog2.webp" />
                                </figure>
                                <div class="pt-8 w-auto">
                                    <h3 class="mt-0.5 text-start container-title-post">
                                        How to position your furniture for positivity
                                    </h3>
                                    <p class="mt-2 line-clamp-3 text-start container-text-post">
                                        Lorem ipsum dolor sit amet, consectetur adipisicing elit.
                                        Recusandae dolores.
                                    </p>
                                </div>
                            </div>
                        </a>
                    </div>
                </div>
            </swiper-slide>
            <swiper-slide class="bg-red-100">
                <div class="w-full">
                    <div class="container-post">
                        <a href="$">
                            <div class="container-img-post">
                                <figure>
                                    <img src="https://handmade.company/goat/img/home/blog/blog1.webp" />
                                </figure>
                                <div class="pt-8 w-auto">
                                    <h3 class="mt-0.5 text-start container-title-post">
                                        How to position your furniture for positivity
                                    </h3>
                                    <p class="mt-2 line-clamp-3 text-start container-text-post">
                                        Lorem ipsum dolor sit amet, consectetur adipisicing elit.
                                        Recusandae dolores.
                                    </p>
                                </div>
                            </div>
                        </a>
                    </div>
                </div>
            </swiper-slide>
      
        </swiper>
        </div>
        
    </div>
</template>



<style scoped>
@font-face {
    font-family: "Axiforma-bold";
    src: url("../assets/fonts/Axiforma-Bold.woff") format("woff");
}

@font-face {
    font-family: "Axiforma-regular";
    src: url("../assets/fonts/Axiforma-Regular.woff") format("woff");
}

@font-face {
    font-family: "Axiforma-medium";
    src: url("../assets/fonts/Axiforma-Medium.woff") format("woff");
}

.btn-more-post {
    border-radius: 50%;
    width: 20px;
    height: 20px;
    background-color: #000;
    position: absolute;
    right: 20px;
    bottom: 20px;
    background: url('https://img.icons8.com/ios-filled/50/null/plus-math.png') no-repeat center center;
}

.container-post {
    padding: 10px;
}

.container-img-post figure {
    position: relative;
    cursor: pointer;
    overflow: hidden;
    width: 100%;
    aspect-ratio: 3/2;
}

.container-img-post figure img {
    width: 100%;
    height: 100%;
    transition: all 200ms ease-out;
    will-change: transform;
    width: 68.9%;
    height: 200.6px;
    object-fit: cover;
    display: absolute;
    width: 100%;
    height: 100%;
    aspect-ratio: 1.5/1;
}

.container-post a:hover img {
    transform: scale(1.05);
}

.container-img-post figure:hover>img {
    transform: scale(1.05);
}


.title {
    font-family: "Axiforma-medium", sans-serif;
    font-size: 4rem;
    font-weight: 500;
    color: #000;
    text-align: initial;
    margin-bottom: 2rem;
    line-height: 60px;
}

.title {
    white-space: pre-wrap;
}

.container-title-post {
    font-family: "Axiforma-regular", sans-serif;
    font-size: 22px;
    font-weight: 500;
}

.container-text-post {
    font-family: "Axiforma-regular", sans-serif;
    font-weight: 400;
    font-size: 14px;
}

/*Pantallas medianas*/
@media (min-width: 640px) {
    .title {
        font-size: 4rem;
        line-height: 60px;
    }
}

/*Pantallas pequeñas*/
@media (min-width: 768px) {
    .title {
        font-size: 4rem;
        line-height: 60px;
    }
}
</style>
