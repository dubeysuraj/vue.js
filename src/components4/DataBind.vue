<template>
    <div>
        <h1 style="white-space: pre-line">{{message}}</h1>
        <textarea type="textarea" v-model="message"/>
    </div>
</template>

<script>
export default {
    name: 'DataBind.vue',
    data(){
        return{
            message: "Hi"
        }
    }
}
</script>