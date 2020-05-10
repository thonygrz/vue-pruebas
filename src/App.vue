<template>
  <v-app>
    <v-card width="400px" class="mx-auto mt-10 rounded-card" color="#F8F8FF">
      <p class="text-center mt-10 caption grey--text">Sign in with</p>
      <v-card-actions class="justify-center">
        <v-btn elevation="10" text color="primary">
          <v-icon left>mdi-facebook</v-icon>
          Facebook
        </v-btn>
        <v-btn elevation="10" text color="primary">
          <v-icon left color="red">mdi-google</v-icon>
          Google
        </v-btn>
      </v-card-actions>
      <p class="text-center caption grey--text">
        Or sign in with credentials
      </p>
      <v-card-text class="text-center">
        <v-form>
          <v-text-field
            label="Email"
            prepend-inner-icon="mdi-email"
            solo
          ></v-text-field>
          <v-text-field
            label="Password"
            :type="showPassword ? 'text' : 'password'"
            prepend-inner-icon="mdi-lock-open"
            :append-icon="showPassword ? 'mdi-eye' : 'mdi-eye-off'"
            @click:append="showPassword = !showPassword"
            solo
          ></v-text-field>
          <v-btn large color="primary">
            Login
          </v-btn>
        </v-form>
      </v-card-text>
      <v-divider></v-divider>
    </v-card>
    <v-card width="400px" class="mx-auto">
      <v-card-actions width="400" class="text-center">
        <v-btn x-small>Forgot password?</v-btn>
        <v-spacer></v-spacer>
        <v-btn x-small>Register</v-btn>
      </v-card-actions>
    </v-card>
  </v-app>
</template>

<script>
// import HelloWorld from "./components/HelloWorld";

export default {
  name: 'App',

  data: () => ({
    checkbox: true,
    showPassword: false
  })
}
</script>
'./components/HelloWorld''App'
