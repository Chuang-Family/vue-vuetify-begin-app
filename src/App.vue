<template>
  <v-app>
   <v-card width="400px" class="mt-5 mx-auto">
     <v-card-title>
      <h1 class="display-1">Login</h1>
     </v-card-title>
       <v-card-text>
         <v-form>
            <v-text-field prepend-icon="mdi-account" clearable label="user name"> 
            </v-text-field>
            <v-text-field
                :type="showPAssword ? 'text' : 'password'"
                label="user password -> Bobo's birthday"
                prepend-icon="mdi-lock"
                :append-icon="showPAssword ? 'mdi-eye' : 'mdi-eye-off'"
                @click:append="showPAssword = !showPAssword"
                />
           
         </v-form>
       </v-card-text>
       <v-divider></v-divider>
       <v-card-actions>
         <v-btn color="success">Register</v-btn>
         <v-spacer></v-spacer>
         <v-btn color="info">Login</v-btn>
       </v-card-actions>
   </v-card>
  </v-app>
</template>
<script>

export default {
  name: 'App',
  data() {
    return {
      showPAssword: false
    }
  },
  components: {
  },
};
</script>
