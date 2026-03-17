<template>
  <div class="d-flex justify-center align-center" style="height: 100vh">

    <v-card width="400"  class="text-center" elevation="11">
      <!-- LOGO -->
       <v-icon size="90" color="pink" class="pt-10">mdi-apple</v-icon>
      <v-card-text class="py-10">
        <!-- Username TextField -->
        <v-text-field variant="outlined" v-model="username" flat label="Username" prepend-inner-icon="mdi-account" clearable></v-text-field>
        <!-- Password TextField -->
        <v-text-field variant="outlined" v-model="password" flat label="Password" prepend-inner-icon="mdi-lock" type="Password" clearable></v-text-field>
        <!-- Signin Button -->
        <v-btn color="primary" @click="login()" block="">Sign In</v-btn>
      </v-card-text>
    </v-card>

  </div>
</template>
<script setup>
definePageMeta({
  layout: 'auth',
});

const defaultUsername = ref("admin");
const defaultPassword = ref("admin123")
const username = ref("")
const password = ref("")


// Regular Function
function login() {
alert ("Login function called ")

}

</script>