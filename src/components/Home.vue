<template>
    <div>
        <!-- <h1 >Hello from Home component</h1> -->
        <!-- <h2>{{data}}</h2>
        <h2>{{msg}}</h2> -->
        <!-- <button v-on:click="Hello('hello call')">Call hello function</button> -->
        <!-- <button v-on:mouseover="Hello('you hover the button')">Call Hello function</button> -->
        <!-- condition rendering -->
        <h1 v-if="show" >condition rendering in vue js</h1>
           <h1 v-else >condition rendering </h1>

           <button v-on:click="display" >Toggle Element</button>

           <table  border="1px">
               <tr>
                   <td>Id</td>
                   <td>Name</td>
                   <td>email</td>
               </tr>
                <tr v-for="user in users" :key="user.id">
                   <td>{{user.id}}</td>
                   <td>{{user.name}}</td>
                   <td>{{user.email}}</td>
               </tr>
               
           </table>
    </div>
</template>

<script>
export default {
    name: "Home",
    props:{
        data:String,
        msg: String
    }, 
    // methods:{
        // Hello(data){
        //     // console.log("Hello function called :)");
        //     // alert("You clicked hello button XD")
        //     alert(data)
        // }
        // display(){
        //     this.show = !this.show
        // }
    // }
    data() {
        // return {show:true}
        return {
            users:[
                {id:1,name:'Suraj',email:'suraj@gmail.com'},
                {id:2,name:'Yuvraj',email:'yuvraj@gmail.com'},
                {id:3,name:'Lalit',email:'lalit@gmail.com'},
                {id:4,name:'Mohit',email:'mohit@gmail.com'},
            ]
        }
    }
};
</script>