<script>
    export default { 
        data() {
            return {
                // Add code here
                id: 'demo1',
                currentColour: 'redBox', //starting with red
                buttonClass: 'btn-danger' //button colour 
            };
        },
        methods: { 
   			// Add code here
            toggleColour(){
                this.currentColour = this.currentColour === 'redBox' ? 'blueBox' : 'redBox';

                this.buttonClass = this.buttonClass === 'btn-primary' ? 'btn-danger' : 'btn-primary';
            }
		}
    };
</script>

<template>
    
    <!-- Modify code here -->
    <div class="container">
        <div v-bind:id="id" v-bind:class="['m-2', currentColour]">
            div ID : {{id}} 
        </div>
        
        <button type="button" class="btn" v-bind:class="buttonClass" v-on:click="toggleColour">Change Color</button>
    </div>

</template>

<style scoped>
    .redBox {
        background-color: red;
    }
    .blueBox {
        background-color: blue;
    }
    #demo1 {
        color: white;
    }
</style>
