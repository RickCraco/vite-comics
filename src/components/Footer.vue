<template>
    <footer>
        <div class="container">
            <div class="row">

                <div class="col-6 py-3 d-flex my-5">
                    <div>
                        <ul class="">
                            <li><h4 class="text-white">Dc Comics</h4></li>
                            <li v-for="item in dc_comics" class="text-white nav-item">{{ item }}</li>
                        </ul>

                        <ul>
                            <li><h4 class="text-white">SHOP</h4></li>
                            <li v-for="item in shop" class="text-white nav-item">{{ item }}</li>
                        </ul>
                    </div>
                    
                    <div>
                        <ul>
                            <li><h4 class="text-white">DC</h4></li>
                            <li v-for="item in dc" class="text-white nav-item">{{ item }}</li>
                        </ul>
                    </div>

                    <div>
                        <ul>
                            <li><h4 class="text-white">SITES</h4></li>
                            <li v-for="item in sites" class="text-white nav-item">{{ item }}</li>
                        </ul>
                    </div>
                </div>

                <div class="col-6 position-relative">
                    <img src="img/dc-logo-bg.png" alt="">
                </div>

            </div>
        </div>
    </footer>
</template>

<script lang="ts">
    export default {
        name: 'Footer',
        data() {
            return {
                dc_comics: [
                    'Characters',
                    'Comics',
                    'Movies',
                    'TV',
                    'Games',
                    'Videos',
                    'News'
                ],
                dc: [
                    'Terms of Use',
                    'Privacy Policy (New)',
                    'Ad Choices',
                    'Advertising',
                    'Jobs',
                    'Subscriptions',
                    'Talent Workshops',
                    'CPSC Certificates',
                    'Ratings',
                    'Shop Help',
                    'Contact Us',
                ],
                sites: [
                    'DC',
                    'MAD Magazine',
                    'DC Kids',
                    'DC Universe',
                    'DC Power Visa'
                ],
                shop: [
                    'Shop DC',
                    'Shop DC Collectibles',
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
    footer{
        background-image: url('img/footer-bg.jpg');
        background-size: 100%;
        background-repeat: no-repeat;
    }
    li{
        list-style: none;
    }
    img{
        position: absolute;
        top: -25%;
        right: -15%;
        width: 100%;
    }
</style>