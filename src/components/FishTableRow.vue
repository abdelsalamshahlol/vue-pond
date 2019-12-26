<template>
    <div>
        <tr @click="updateDescriptionState">
            <td class="fish-name">{{fishData.name}}</td>
            <td>
                <img :src="fishData.image"/>
            </td>
            <td class="fish-description" v-if="showDescription">{{fishData.description}}</td>
        </tr>
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