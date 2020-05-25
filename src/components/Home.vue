<template>
  <v-container fluid id="content">
    <div class="page_title">
       <h1> TRACK YOUR PROGRESS/GROWTH DURING YOUR INTERNSHIP. MAINTAIN A CONSTRUCTIVE COMMUNICATION BETWEEN EVERYONE INVOLVE.  </h1>
    <v-divider
          class="mx-4"
          inset true
          horizontal
        ></v-divider>
    </div>
  <v-row class="text-center"  align="center"
          justify="space-between">
      <v-card
      color="blue lighten-5"
      class="mx-auto my-12"
      max-width="374"
      align-center
      >
      <v-card-title primary-title class="justify-center">
        <p class="headline ">STUDENT</p>
      </v-card-title >
      <v-img
        height="300"
        src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=500&q=60"
      ></v-img>
  
  
      <v-card-text>
  
        <div class="my-4 subtitle-1">
           • Blablablablablabla
        </div>
  
        <div>Curabitur tellus magna, porttitor a, commodo a, commodo in, tortor. 
          Donec interdum. Praesent scelerisque. Maecenas posuere sodales odio. 
          Vivamus metus lacus, varius quis, imperdiet quis, rhoncus a, turpis. 
          Etiam ligula arcu, elementum a, venenatis quis, sollicitudin sed, metus. 
          Donec nunc pede, tincidunt in, venenatis vitae, faucibus vel, nibh. Pellentesque wisi. 
          Nullam malesuada.</div>
      </v-card-text>  
  
      <v-card-actions>
         <v-spacer></v-spacer>
        <v-btn href="/signup" color="indigo accent-3" fab dark>
                <v-icon>mdi-account-circle</v-icon>
              </v-btn>

        <v-spacer></v-spacer>
      </v-card-actions>
    </v-card>

    <v-card
      class="mx-auto my-12"
      max-width="374"
      color="blue lighten-5"
    >
     <v-card-title primary-title class="justify-center">
    <p class="headline ">SCHOOL</p>
</v-card-title>
      <v-img
        height="300"
        src="https://images.unsplash.com/photo-1543505298-b8be9b52a21a?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=500&q=60"
      ></v-img>

      <v-card-text>
        <div class="my-4 subtitle-1">
           • Blablablablablablabla
        </div>
  
        <div>Curabitur tellus magna, porttitor a, commodo a, commodo in, tortor. 
          Donec interdum. Praesent scelerisque. Maecenas posuere sodales odio. 
          Vivamus metus lacus, varius quis, imperdiet quis, rhoncus a, turpis. 
          Etiam ligula arcu, elementum a, venenatis quis, sollicitudin sed, metus. 
          Donec nunc pede, tincidunt in, venenatis vitae, faucibus vel, nibh. Pellentesque wisi. 
          Nullam malesuada.</div>
      </v-card-text>
     
  
       <v-card-actions>
         <v-spacer></v-spacer>
       <v-btn color="indigo accent-3" fab dark>
                <v-icon>mdi-account-circle</v-icon>
              </v-btn>

        <v-spacer></v-spacer>
      </v-card-actions>
    </v-card>
    <v-card
      class="mx-auto my-12"
      max-width="374"
      color="blue lighten-5"
    >
    <v-card-title primary-title class="justify-center">
    <p class="headline">COMPANY</p>
</v-card-title>
      <v-img
        height="300"
        src="https://images.unsplash.com/photo-1552664730-d307ca884978?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=500&q=60"
      ></v-img>
  
  
      <v-card-text>
        <!-- <v-row
          align="center"
          class="mx-0"
        >
          <v-rating
            :value="4.5"
            color="amber"
            dense
            half-increments
            readonly
            size="14"
          ></v-rating>
  
          <div class="grey--text ml-4">4.5 (413)</div>
        </v-row> -->
  
        <div class="my-4 subtitle-1">
           • Blablablablabla
        </div>
  
        <div>
          Curabitur tellus magna, porttitor a, commodo a, commodo in, tortor. 
          Donec interdum. Praesent scelerisque. Maecenas posuere sodales odio. 
          Vivamus metus lacus, varius quis, imperdiet quis, rhoncus a, turpis. 
          Etiam ligula arcu, elementum a, venenatis quis, sollicitudin sed, metus. 
          Donec nunc pede, tincidunt in, venenatis vitae, faucibus vel, nibh. Pellentesque wisi. 
          Nullam malesuada.
        </div>
      </v-card-text>
        
      <v-card-actions>
         <v-spacer></v-spacer>
        <v-btn color="indigo accent-3" fab dark>
                <v-icon>mdi-account-circle</v-icon>
              </v-btn>
        <v-spacer></v-spacer>
      </v-card-actions>
    </v-card>
     </v-row>
  </v-container>
</template>

<script>
  export default {
    name: 'Home',
    data () {
      return {
         alignment: 'center',
      dense: false,
      justify: 'center',
      }
    },
  }
</script>
<style lang="scss">
.page_title{
  margin-top: 3%;
  margin-bottom: 1%;
  text-align: center;
}
</style>
