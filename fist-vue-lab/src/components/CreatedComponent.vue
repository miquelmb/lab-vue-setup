<template>
    <div>
        <div id="lab1-iteration2-text-interpolation">
            <h1>This is {{myName}}'s first Vue.js lab at Ironhack Bootcamp</h1>
        </div>

        <br>
        
        <div id="lab-1-bonus-hello-world-button">
            <button v-on:click="helloWorld()">Click Me</button>
        </div>

        <br>

        <div id="lab-2-iteration-2">
            <h2>Lab-2 Iteration 2. The result of the operation is: {{jsOperation()}}</h2>
        </div>

        <br>

        <div id="lab-2-iteration-3">
            <h2 v-show="iteration2Show">It's happening, i'm beeing shown!</h2>
        </div>

        <br>

        <div id="lab2-iteration4">
            <h2 v-for="(person, index) in iteration4data" v-bind:key="person">
            {{ index +1 }}- {{ person.shortName }}. Job: {{person.job}} - {{person.hoursPerDay}} per day</h2>
        </div>

        <br>

        <div :style="styleBackground" id="-lab2-iteration5">With this color you can see me!</div>

        <div id="lab2-bonus-iteration5">
            <button v-on:click="changeBackground()">Change above div color</button>
        </div>

        <br>
    </div>
    
</template>

<script>
// import { builtinModules } from 'module'



export default {
    name: 'CreatedComponent',
    data () {
        return {
            myName: "Miquel",

            iteration2Show: true,

            iteration4data: [
                {
                shortName: "Josh",
                job: "UX",
                hoursPerDay: "8hrs"
                },
                {
                shortName: "Carla",
                job: "UI",
                hoursPerDay: "6hrs"
                },
                {
                shortName: "Phil",
                job: "Front-End Dev",
                hoursPerDay: "10hrs"
                }
            ],

            styleBackground: {
                backgroundColor: "#2c3e50",
            }

        
        }
    },
    methods: {
        helloWorld() {
            console.log('Hello World!')
        },

        jsOperation() {
            return 2**4
        },

        changeBackground() {
            this.styleBackground.backgroundColor = "lightgreen"
        }
    }
}
</script>