<template>
    <div id="fish">
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
    #fish:hover {
        animation: float 0.9s forwards ease-in-out ;
    }

    @keyframes float {
        0% {
            opacity: 0.5;
            transform: scale(1);
        }
        100%{
            opacity: 1;
            transform: scale(1.1);
        }
    }
</style>