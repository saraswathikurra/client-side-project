<template>
   <article>
        <div class="Login" :class="{'sign-up-active' : signUp}"> 
            <div class="overlay-Login">
                <div class="overlay">
                    <div class="overlay-left">
                        <h2>Welcome Back!</h2>
                        <p>Please Sign in if you already have an account</p>
                        <router-link to="/signin" tag="button">Sign In</router-link>
                    </div>
                    <div class="overlay-right">
                        <h2></h2>
                        <p>Create an account if you do NOT have an account in Better health</p>
                        <router-link to="/signup" tag="button">Sign Up</router-link>
                    </div>
                </div>
            </div>
            
        </div>
    </article>
</template>

