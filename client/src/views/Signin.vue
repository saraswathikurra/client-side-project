<template>
  <div class="Signin">
    <h1>This is an Sign in page</h1>
    <form class="sign-in" action="#">
                <h2>Sign In</h2>
                <div>Use your account</div>
                Email-ID: <br>
                <input type="email" name = "email" v-model="input.email" placeholder="Email" />
                <br>
                <br>
                Password: <br>
                <input type="password" name = "password" v-model="input.password" placeholder="Password" />
                <br>
                <br>
                <a href="#">Forgot your password?</a>
                <br>
                <br>
                <button type = "button" v-on:click="login_verification()">Sign In</button>
                <p >{{greetings}} </p>
                
            </form>
  </div>
</template>
<script>
import json from './../data/login.json';

console.log("first_name"+json[0].email);

  export default {
    name: 'Sign In',
    data(){
      return{
        input:{
          email: "",
          password: ""
        }
      }
    },
    methods: {
      login_verification(){
        console.log("inside login.verfication NOW")
        console.log("jsonlenght " + json.length);
        var json_length = json.length;
        for(var i = 0 ;i <json_length; i++){
          if(this.input.email == json[i].email && this.input.password == json[i].password){
          console.log("SUCESSSSSSS");
          this.$router.push({name: 'Signedinpage', query:{redirect:'/signedinpage'}})
        }
        else{
          console.log("FAILLLL");
        }
        }
        
      }
    }
  }

</script>

