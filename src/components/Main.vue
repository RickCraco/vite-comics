<template>
    <nav>
        <div class="py-4 text-white boack">
            <section class="w-100 sezione-top position-relative">
                <h3 class="bg-primary text-white text-uppercase p-3">Current series</h3>
            </section>
            <section>
                <div class="container py-5">
                    <div class="row">
                        <Card v-for="item in comics" :thumbs="item.thumb" :title="item.series"/>
                    </div>
                </div>
            </section>
        </div>
        <div class="my-bg" id="div-blu ">
            <div class="container">
                <div class="d-flex nav align-items-center justify-content-center">
                    <div class="px-3 nav-item d-flex align-items-center py-4" v-for="item in menu">
                        <div><img :src="item.img" alt=""></div>
                        <span class="px-2 text-white">{{ item.text }}</span>
                    </div>
                </div>
            </div>
        </div>
    </nav>
</template>

<script lang="ts">
import axios from 'axios';
import Card from './Card.vue';

export default {
    name: 'Main',
    components: {
        Card,
    },
    data() {
        return {
            comics:[],
            menu: [
                {
                    text: 'DIGITAL COMICS',
                    img: 'img/buy-comics-digital-comics.png',
                },
                {
                    text: 'DC MERCHANDISE',
                    img: 'img/buy-comics-merchandise.png',
                },
                {
                    text: 'SUBSCRIPTION',
                    img: 'img/buy-comics-subscriptions.png',
                },
                {
                    text: 'COMIC SHOP LOCATOR',
                    img: 'img/buy-comics-shop-locator.png',
                },
                {
                    text: 'DC POWER VISA',
                    img: 'img/buy-dc-power-visa.svg',
                },
            ]
        }
    },
    mounted(){
        axios.get('dc-comics.json').then(el =>{
            this.comics = el.data;
        })
    }
}
</script>

<style lang="scss" scoped>
.boack {
    background-color: black;
}

.my-bg {
    background-color: rgb(18, 146, 231);
}

img {
    width: 50px;
    height: 65px;
}

nav {
    position: relative;
    z-index: 1000;
}

.sezione-top {
    height: 40vh;
    background-image: url('img/jumbotron.jpg');
    background-size: 100%;
}

h3{
    position: absolute;
    bottom: -10%;
    left: 22%;
    z-index: 5000;
}
</style>