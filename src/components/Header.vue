    <template>
      <v-app-bar
      app
      shrink-on-scroll
      dark
    >
    <v-spacer></v-spacer>
      <div class="d-flex align-center">
        <v-img
          :src="image"
          class="shrink mr-2"
          contain
          transition="scale-transition"
          width="150"
        />
      </div>

      <v-spacer></v-spacer>
      </v-app-bar>
</template>
<script>
export default {
     data () {
  return {
    image: require('@/assets/Logo2.png')
  }
},
}
</script>>