<template>
    <div class="py-4 text-white boack">
        <div class="container">
            <h1>--&gt;Content goes here &lt;--</h1>
        </div>
    </div>
    <div class="my-bg">
        <div class="container">
            <ul class="d-flex nav align-items-center justify-content-center">
                <li class="px-3 nav-item" v-for="item in menu">
                    <img :src="item.img" alt="">
                    {{ item.text }}
                </li>
            </ul>
        </div>
    </div>
</template>

<script lang="ts">
    export default {
        name: 'Main',
        data() {
            return {
                menu:[
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
        }
    }
</script>

<style lang="scss" scoped>
.boack{
    background-color: black;
}

.my-bg{
    background-color: rgb(18, 146, 231);
}

img{
    width: 25%;
}
</style>