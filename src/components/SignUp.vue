<template>
    <div>
        <input type="text" placeholder="enter your name" v-model="signup.username" /> <br> <br>
        <input type="text" placeholder="enter your password" v-model="signup.password" /> <br> <br>
        <p>Choose Hobbies</p>
        <input type="checkbox" id="cricket" value="cricket" v-model="signup.hobbies" />
        <label for="cricket">Cricket</label>
        <input type="checkbox" id="football" value="football" v-model="signup.hobbies" />
        <label for="football">Football</label> <br> <br>
        <p>Select Gender</p>
        <input type="radio" id="female" value="female" v-model="signup.gender" />
        <label for="female">Female</label>
         <input type="radio" id="male" value="male" v-model="signup.gender" />
        <label for="male">Male</label>
        <br> <br>
        <button v-on:click="signupUser">Sign Up</button>
    </div>
</template>
<script>
export default {
    name: 'SignUp',
    data(){
        return{
            signup:{
                username: null,
                password: null,
                hobbies: [],
                gender: null
            }
        }
    },
    methods: {
        signupUser(){
            console.warn(this.signup)
        }
    },
}
</script>