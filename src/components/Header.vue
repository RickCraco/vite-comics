<template>
    <header>
        <div class="container d-flex align-items-center justify-content-between py-3">
            <img src="../../public/img/dc-logo.png" alt="logo">
            <ul class="d-flex nav">
                <li class="px-3 nav-item" v-for="item in menu">{{ item.text }}</li>
            </ul>
        </div>
    </header>
</template>

<script lang="ts">
    export default {
        name : 'Header',
        data(){
            return {
                menu : [
                    {
                        text: 'CHARACTERS',
                        id: 1
                    },
                    {
                        text: 'COMICS',
                        id: 2
                    },
                    {
                        text: 'MOVIES',
                        id: 3
                    },
                    {
                        text: 'TV',
                        id: 4
                    },
                    {
                        text: 'GAMES',
                        id: 5
                    },
                    {
                        text: 'COLLECTIBLES',
                        id: 6
                    },
                    {
                        text: 'VIDEOS',
                        id: 7
                    },
                    {
                        text: 'FANS',
                        id: 8
                    },
                    {
                        text: 'NEWS',
                        id: 9
                    },
                    {
                        text: 'SHOP',
                        id: 10
                    },
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
</style>