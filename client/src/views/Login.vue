<template>
   <article>
        <div class="Login" :class="{'sign-up-active' : signUp}"> 
            <div class="overlay-Login">
                <div class="overlay">
                    <div class="overlay-left">
                        <h2>Sign into your account</h2>
                        <h2>with your credentials!</h2>
                        <router-link to="/signin" tag="button">Sign In</router-link>
                    </div>
                    <div class="overlay-right">
                        <h2>Click the SignUp button to REGISTER!</h2>
                        <router-link to="/signup" tag="button">Sign Up</router-link>
                    </div>
                </div>
            </div>
            
        </div>
    </article>
</template>

