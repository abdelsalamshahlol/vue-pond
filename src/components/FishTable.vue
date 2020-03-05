<template>
    <div id="wrapper">
        <FishTableRow v-for="(fish, index) in fishes" :fish="fish" :key="index"/>
    </div>
</template>

<script>
    import FishTableRow from './FishTableRow.vue';

    export default {
        name: "FishTable",
        components: {
            FishTableRow
        },
        props: ['fishes'],
    }
</script>

<style scoped>
    #wrapper {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }
</style>