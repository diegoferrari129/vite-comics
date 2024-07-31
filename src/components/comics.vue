<script>
export default {
    props: {
        contentImg: String,
        contentTitle: String

    },
}
</script>

<template>

<div class="col-2">
    <div class="main__content">
        <img :src="contentImg" :alt="contentTitle">
    </div>
    <h6>{{contentTitle}}</h6>
</div>

</template>

<style lang="scss" scoped>
.main__content {
    padding-top: 40px;
    display: flex;
    width: 170px;
    height: 200px;

    img {
        object-fit: cover;
        object-position: top;
        width: 100%;
        height: 100%;
    }
}

h6 {
    padding-top: 10px;
}

</style>