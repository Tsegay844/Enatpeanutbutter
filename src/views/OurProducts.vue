<template>
  <div class="home">
    <v-card :class="['card', `card--${$vuetify.breakpoint.name}`]" :style="{
      backgroundImage: `url(${bgImage})`,
      backgroundSize: 'cover',
      backgroundPosition: 'center',
      width: '100%',
      display: flex, justify: center
    }">
      <v-container fluid>
        <v-card-title :class="{
          'card-title-xs': $vuetify.breakpoint.xsOnly,
          'card-title-sm': $vuetify.breakpoint.smAndUp,
          'card-title-md': $vuetify.breakpoint.mdAndUp,
        }" style="color:whitesmoke">
          <span> <Strong>Products we Offer</Strong></span>
        </v-card-title>
      </v-container>
      <v-divider height="5px" color="dimgrey" />
    </v-card>
    <v-card class="mx-auto"
    max-width="1250"
    flat>
    <v-divider height="5px" color="dimgrey" />
    <v-card flat
    height="20px"></v-card> 
      <h3 style="color:dimgray">Experts in Peanut Butter</h3>
      <v-card flat
    height="8px"></v-card>
      <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Assumenda molestiae, unde temporibus nam omnis soluta dolore tempora est at aperiam culpa, nihil laboriosam aut modi quas id aspernatur impedit similique!</p>
      <v-container fluid>
      <v-row dense>
        <v-col
        cols="12" xs="12" sm="6" md="4" lg="3"
          v-for="bodyImage in bodyImages"
          :key="bodyImage.title"
        >
          <v-card>
            <v-img
              :src="bodyImage.src"
              class="align-end"
              gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
              height="220px"
              cover
            >  
            </v-img>
            <P class="text-8 text-italic text-center" > {{bodyImage.title}}</p>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
    </v-card>       
  </div>
</template>
<script>
export default {
  data: () => ({
    cards: [
      { title: 'Pre-fab homes', src: require("../assets/p.jpg"), flex: 12 },
      { title: 'Favorite road trips', src: 'https://cdn.vuetifyjs.com/images/cards/road.jpg', flex: 2 },
      { title: 'Best airlines', src: 'https://cdn.vuetifyjs.com/images/cards/plane.jpg', flex: 6 },
    ],
    bodyImages: [
        {  title: '1kg', src: require("../assets/p1kg.jpg") },
        {  title: '60g', src: require("../assets/p0.6kg.jpg") },
        {  title: '4g', src: require("../assets/p0.4kg.jpg") },
        {  title: 'እናት መዳፈ', src: require("../assets/pmedafe.jpg") }, 
      ],
    bgImage: require("../assets/bg1.jpg"),
    title: 'Card Title',
    text: 'Card content here'
  }),
}
</script>
<style>
.home {
  margin-top: 65px;
}

.card-title-xs {
  font-size: 16px;
}

.card-title-sm {
  font-size: 24px;
}

.card-title-md {
  font-size: 28px;
}

.card-title-lg {
  font-size: 32px;
}

.card-text-xs {
  font-size: 16px;
}

.card-text-sm {
  font-size: 18px;
}

.card-text-md {
  font-size: 20px;
}

.card-text-sm {
  font-size: 22px;
}
.body{
  margin-left: 200px;
  margin-right: 200px;
}
.text-10 {
  font-size: 5px !important;
}

.text-italic {
  font-style: italic !important; 
}

.text-center {
  text-align: center !important;
}


</style>
