<template>
    <div id="iteration2-text-interpolation">
        <h1>This is {{myName}}'s first Vue.js lab at Ironhack Bootcamp</h1>
    </div>
</template>

<script>
export default {
    name: 'CreatedComponent',
    data () {
        return {
            myName: "Miquel"
        }
    }
}
</script>