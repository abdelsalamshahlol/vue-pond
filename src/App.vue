<template>
    <div id="app">
        <FishTable :fishes="fishData"/>
    </div>
</template>

<script>
    import FishTable from './components/FishTable.vue';

    export default {
        name: 'app',
        components: {
            FishTable
        },
        data() {
            return {
                fishData : [
                    {
                        name: 'Goldfish',
                        image: 'http://tinyurl.com/n4vgcl5',
                        description: 'Everyone\'s first pet'
                    },
                    {
                        name: 'Pufferfish',
                        image: 'http://tinyurl.com/kxd7cuu',
                        description: 'So puffy!'
                    },
                    {
                        name: 'Tuna',
                        image: 'http://tinyurl.com/zgs7z2s',
                        description: 'Why are these things so huge? THey\'re terrifying.'
                    }
                ]
            }
        }
    }
</script>

<style>
    #app {
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        margin-top: 60px;
        background: #0073aa;
        padding: 5rem;
        color: #fefeff;
        font-size: 25px;
        font-family: monospace;
        border: 2px solid #bdbdbd;
        box-shadow: 1px 1px 7px 2px #928b8b;
    }
</style>
