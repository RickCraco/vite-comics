<template>
    <header>
        <div class="container d-flex align-items-center justify-content-between py-3">
            <img src="../../public/img/dc-logo.png" alt="logo">
            <ul class="d-flex nav">
                <li class="px-3 nav-item" v-for="item in menu">{{ item }}</li>
            </ul>
        </div>
    </header>
</template>

<script lang="ts">
    export default {
        name : 'Header',
        data(){
            return {
                menu : ['CHARACTERS','COMICS','MOVIES', 'TV','GAMES','COLLECTIBLES', 'VIDEO','FANS','NEWS', 'SHOP']
            }
        }
    }
</script>

<style lang="scss" scoped>
</style>