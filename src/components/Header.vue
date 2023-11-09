<template>
    <header>
        <div class="container">
            <img src="../../public/img/dc-logo.png" alt="logo">
            <ul>
                <li></li>
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