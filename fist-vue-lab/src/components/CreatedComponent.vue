<template>
    <div>
        <div id="iteration2-text-interpolation">
        <h1>This is {{myName}}'s first Vue.js lab at Ironhack Bootcamp</h1>
    </div>

    <div id="hello-world-button">
        <button v-on:click="helloWorld()">Click Me</button>
    </div>
    </div>
    
</template>

<script>


export default {
    name: 'CreatedComponent',
    data () {
        return {
            myName: "Miquel",
        }
    },
    methods: {
        helloWorld() {
            console.log('Hello World!')
        },
    }
}
</script>