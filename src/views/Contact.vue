<template>
  <div class="contact">
    <v-row justify="center">
    <v-col
      cols="12"
      sm="8"
    >
      <v-card>
        <v-card-title class="cyan darken-1" :style="{ background: 'url(' + imageSrc + ')' }">
          <span class="text-h5 white--text"><Strong>Contact us</Strong> </span>
          <v-spacer></v-spacer> 
        </v-card-title>
      <v-card flat height="15px"></v-card>
        <p>We want to hear from you!<br> 
Would you like to send feedback on our product?<br>
Use the following addresses to reach us. Our customer response team is ready to serve you!</P>
        <v-list>
          <v-list-item>
            <v-list-item-action>
              <v-icon>mdi-phone</v-icon>
            </v-list-item-action>
            <v-list-item-content>
              <v-list-item-title>+251912388296</v-list-item-title>
            </v-list-item-content>
            <v-list-item-action>
              <v-icon>mdi-message-text</v-icon>
            </v-list-item-action>
          </v-list-item>

          <v-divider inset></v-divider>

          <v-list-item>
            <v-list-item-action>
              <v-icon>mdi-phone</v-icon>
            </v-list-item-action>
            <v-list-item-content>
              <v-list-item-title>+251914892551</v-list-item-title>
            </v-list-item-content>
            <v-list-item-action>
              <v-icon>mdi-message-text</v-icon>
            </v-list-item-action>
          </v-list-item>

          <v-divider inset></v-divider>

          <v-list-item>
            <v-list-item-action>
              <v-icon>mdi-email</v-icon>
            </v-list-item-action>

            <v-list-item-content>
              <v-list-item-title> enatpeanutbutter@gmail.com</v-list-item-title>
            </v-list-item-content>
          </v-list-item>

          <v-divider inset></v-divider>

          <v-list-item>
            <v-list-item-action>
              <v-icon>mdi-map-marker</v-icon>
            </v-list-item-action>

            <v-list-item-content>
              <v-list-item-title>Mekelle, Ethiopia</v-list-item-title>
            </v-list-item-content>
          </v-list-item>
        </v-list>

        <v-img
          
          height="50px"
        ></v-img>
      </v-card>
    </v-col>
  </v-row>
  </div>
</template>
<style>
.contact{
  margin-top: 65px;
}
</style>

<script>
export default {
  data () {
  return {
    imageSrc: require("../assets/bg1.jpg"),
  }
} 
}
</script>