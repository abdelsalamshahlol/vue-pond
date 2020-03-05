<template>
    <div>
        <div @click="updateDescriptionState">
            <div class="fish-name">{{fishData.name}}</div>
            <div>
                <img :src="fishData.image"/>
            </div>
            <span class="fish-description" v-if="showDescription">{{fishData.description}}</span>
        </div>
    </div>
</template>

<script>
    export default {
        name: "FishTableRow",
        props: ['fish'],
        data() {
            return {
                fishData: this.fish,
                showDescription: false
            }
        },
        methods: {
            updateDescriptionState() {
                this.showDescription = !this.showDescription;
            }
        }
    }
</script>

<style scoped>

</style>