<template>
    <div class="col-2">
        <img :src="thumbs" :alt="title" class="card-img-top ">
        <div>
            <h5>{{ title }}</h5>
        </div>
    </div>
</template>

<script lang="ts">
    export default {
        name: 'Card',
        props:['thumbs','title']
    }
</script>

<style lang="scss" scoped>
    img{
        width: 200px;
        height: 200px;
    }
    h5{
        font-size: 15px;
    }
</style>