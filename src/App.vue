<template>
  <div id="app">
      <v-app id="inspire">
      <HeaderNav/>
<v-content>
    <router-view/>
  </v-content>
    </v-app>
<FooterNav/>
  </div>
</template>
<script>
import HeaderNav from './components/Header';
import FooterNav from './components/Footer';
export default {
  name: 'App',

  components: {
    HeaderNav,
    FooterNav
  },

  data () {
  return {
    
  }
},
};
</script>

