<script>
    export default { 
        // Add Code Here
        data(){
            return{
                message: 'Choose your favourite fruit:',
                fruitsArray: ['apple', 'orange', 'peach'],
                selectedFruit: ''
            };
        },
        // challenge: use array 
        computed: {
            fruit1(){
                return this.fruitsArray[0];
            },

            fruit2(){
                return this.fruitsArray[1];
            },

            fruit3(){
                return this.fruitsArray[2];
            }
        },
        methods: {}

    };
</script>

<template>
    <div id="app">
        {{ message }} </br>
        {{ fruit1 }} <input type="radio" name="fruit">
        {{ fruit2 }} <input type="radio" name="fruit">
        {{ fruit3 }} <input type="radio" name="fruit">
    </div>
</template>

<style scoped>
</style>
