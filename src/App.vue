<template>
    <div id="app">
        <!--<img alt="Vue logo" src="./assets/logo.png">-->
        <!--<HelloWorld msg="Welcome to Your Vue.js App"/>-->
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
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;
        margin-top: 60px;
    }
</style>
