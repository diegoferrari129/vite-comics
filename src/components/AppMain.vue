<script>
import contentMain from '../data/dc-comics.json';
import comics from './comics.vue';
export default {

    components: {
        comics
    },
    data() {
        return {
            contentMain: contentMain
        }
    },
}
</script>

<template>
    <div class="jumbotron">
        <div class="row"></div>
    </div>
    <main class="main">
        <div class="container">
            <div class="row">
                <comics v-for="content in contentMain" key="c-`${content.id}`" :contentImg="content.thumb" :contentTitle="content.series"/>
            </div>
        </div>
    </main>
</template>

<style lang="scss" scoped>
    .jumbotron {
        background-image: url(../assets/img/jumbotron.jpg);
        background-size: cover;
        min-height: 400px;
    }

    .main {
        background-color: black;
        color: white;
        padding-bottom: 40px;
    }

</style>