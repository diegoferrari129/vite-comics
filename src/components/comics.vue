<script>
export default {
    props: {
        contentImg: String,
    },
}
</script>

<template>

    <div class="col-2">
        <div class="main__content">
            <img :src="contentImg" :alt="contentTitle">
            <h6>{{contentTitle}}</h6>
        </div>
    </div>

</template>

<style lang="scss" scoped>
    
</style>