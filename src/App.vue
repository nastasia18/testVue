<template>
  <v-app>
    <HeaderComponent></HeaderComponent>
    <v-main>
      <v-container>
        <CafeComponent></CafeComponent>
      </v-container>
    </v-main>
    <FooterComponent></FooterComponent>
  </v-app>
</template>

<script>
import CafeComponent from './components/Cafe.vue';
import HeaderComponent from './components/Header.vue';
import FooterComponent from './components/Footer.vue';

export default {
  name: 'App',

  components: {
    CafeComponent,
    HeaderComponent,
    FooterComponent
  },

  data: () => ({
    //
  }),
};
</script>