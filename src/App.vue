<template>
  <v-app>
    <v-app-bar app color="primary" dark >
    </v-app-bar>
      <v-main class="text-center">
        <Login v-if="true"/>
        <ForgotPassword v-if="false"/>
        <Register v-if="false"/>
        
        
        <!-- <v-container align="center" justify="center">
          <v-row align="center" justify="center" dense>
                <v-col cols="12" sm="8" md="4" lg="4">
                    <v-card elevation="0">
                    <a href="http://localhost:8080/">
                        <v-img 
                            src="@/assets/logo.svg" 
                            alt="logo" contain height="50"></v-img>
                    </a>
                    <h1>Reaction Time</h1>
                    <v-card-text>
                        <v-card-actions class="text--secondary">
                            <v-btn @click="start"
                            x-large block dark  elevation="2">Play</v-btn>
                        </v-card-actions>
                    </v-card-text>
                    </v-card>
                </v-col>
            </v-row>
        </v-container> -->
        

      </v-main>
  </v-app>
</template>

<script>
import Login from './components/Login.vue';
import ForgotPassword from './components/ForgotPassword.vue';
import Register from './components/Register.vue';

export default {
  name: 'App',
  components: { 
    Login,
    ForgotPassword,
    Register
  },
  data: () => ({
    isPlaying: false,
    delay: null
  }),
  // data(){
  //   return {
  //   isPlaying: false,
  //   delay: null 
  //   }
  // },
  // methods: {
  //   start(){
  //     this.delay = 2000
  //     this.isPlaying = true
  //   }
  // }
};
</script>
