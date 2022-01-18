<template>
   <div>
        <h1 class="Home">Class and Style Bindings</h1>
        <h1 v-bind:style="{color: colorKey}">Style Bindings</h1>
        <h1 v-bind:class="{display:show}">Class binding with objects</h1>
        <h1 v-bind:class="[show ? 'yesShow': 'noShow']">class bindings with array</h1>
   </div>
</template>

<script>
export default {
    name: 'Home',
    data(){
        return{
            show:true,
            aclass: 'arrayClass',
            colorKey: 'red'
        }
    }
}
</script>

<style scoped>
     .Home{
         color: orange
     }
     .display{
         background-color: yellow;
     }
     .arrayClass{
         color: greenyellow;
     }
</style>