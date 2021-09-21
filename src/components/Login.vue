<template>
    <v-app>
        <v-main>
        <v-container class="fill-height" fluid>
            <v-row align="center" justify="center" dense>
                <v-col cols="12" sm="8" md="4" lg="4">
                    <v-card elevation="0">
                    <a href="http://localhost:8080/">
                        <v-img 
                            src="@/assets/logo.svg" 
                            alt="logo" contain height="200"></v-img>
                    </a>
                    <v-card-text>
                        <v-form>
                        <v-text-field 
                            label="Enter your email" 
                            name="email" 
                            prepend-inner-icon="mdi-email" 
                            type="email" outlined></v-text-field>
                        <v-text-field 
                            label="Enter your password" 
                            name="password" 
                            prepend-inner-icon="mdi-lock" 
                            type="password" 
                            suffix="| Forgot?" outlined></v-text-field>
                        <v-btn 
                            class="rounded-0" 
                            x-large block dark  elevation="2">Login</v-btn>
                        <v-card-actions class="text--secondary">
                            <v-checkbox label="Remember me"></v-checkbox>
                            <v-spacer></v-spacer>
                            <!-- <router-link :to="{ name: 'SignUp' }">Sign Up</router-link> -->
                            No account? <a href="#" class="pl-2" style="color: #000000">Sign Up</a>
                        </v-card-actions>
                        </v-form>
                    </v-card-text>
                    </v-card>
                </v-col>
            </v-row>
        </v-container>
        </v-main>
  </v-app>
</template>

<script>
export default {
    name: 'Login'
}
</script>

<style lang="css" scoped>
</style>