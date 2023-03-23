<template>
  <v-app>
    <v-app-bar
      app
      
      
    >
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="@/assets/Librarian_Woman.jpg"
          transition="scale-transition"
          width="40"
        />

        {{ $const.APP_NAME }}
      </div>

      <v-spacer></v-spacer>

      <v-btn
        href="https://accounts.google.com/v3/signin/identifier?dsh=S1107838969%3A1678948649108238
        &continue=https%3A%2F%2Fmail.google.com%2Fmail%2Fu%2F0%2F&
        emr=1&followup=https%3A%2F%2Fmail.google.com%2Fmail%2Fu%2F0%2F&
        ifkv=AWnogHd5qp3P4Y1gn1pmDio8qsRdcpzYJjF0xs2frUEpFWtc60btg2tEEXPUOi0HVPI4aHkz9biB&
        osid=1&passive=1209600&service=mail&flowName=GlifWebSignIn&flowEntry=ServiceLogin"
        target="_blank"
        text
      >
        <span class="mr-2">LOGIN</span>
        <v-icon>mdi-account-circle</v-icon> <!-- sourced this from 
                                            VUE documentation app -->
      </v-btn>
    </v-app-bar>

    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script>

export default {
  name: 'App',

  data: () => ({
    //
  }),
};
</script>

<style>
@import url('@/assets/styles.css');
</style>