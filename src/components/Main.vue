<template>
    <nav>
        <div class="py-4 text-white boack">
            <div class="container">
                <h1>--&gt;Content goes here &lt;--</h1>
            </div>
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
export default {
    name: 'Main',
    data() {
        return {
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
</style>