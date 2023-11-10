<template>
    <div class="card">
        <img :src="thumbs" :alt="title" class="card-img-top">
        <div class="card-body">
            <h5 class="card-title">{{ title }}</h5>
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

</style>