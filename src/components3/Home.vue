<template>
    <div>
        <h1>This is Home Component</h1>
        <p v-html="rowHtml"></p>
        <h3 v-once>{{name}}</h3>
        <h3>{{name}}</h3>

        <h3>{{ok ? "Yes" : "No"}}</h3>
        <button v-bind:disabled="disableBtn" v-on:click="updateText">Click me</button>
    </div>
</template>

<script>
export default {
    name: 'Home',
    data(){
        return{
            name: 'Suraj',
            a:10,
            b:20,
            ok:false,
            rowHtml: "<h1>Suraj is Here</h1>",
            disableBtn: false
        }
    },
    methods: {
        updateText(){
                this.name="Selena"
                this.ok=!this.ok
          
        }
    } , 
}
</script>