<template>
 <v-container fluid>
   <div class="page_title">
       <h1> CREATE YOUR STUDENT PROFILE </h1>
       <v-row align="" justify="center">
           <v-avatar color="grey" size="200">
        <v-icon dark size="50">mdi-account-circle</v-icon>
      </v-avatar>
        
       </v-row>
       <v-row align="center" justify="center">
           <v-btn
        :loading="loading3"
        :disabled="loading3"
        color="blue-grey"
        class="ma-2 white--text"
        @click="loader = 'loading3'"
      >
        Upload a picture
        <v-icon right dark>mdi-cloud-upload</v-icon>
      </v-btn>
       </v-row>
    <v-divider
          class="mx-4"
          inset true
          horizontal
        ></v-divider>
    </div>
  <v-row align="center" justify="center">
      <v-form >
        <v-row justify="center">
        <h2 class="text-align">Personal contact informations</h2>
        </v-row>
        
        <v-text-field
          v-model="Firstname"
          :rules="nameRules"
          label="Firstname*"
          required
        ></v-text-field>

        <v-text-field
          v-model="Lastname"
          :rules="nameRules"
          label="Lastname*"
          required
        ></v-text-field>
        
        <v-text-field
          v-model="Country"
          :rules="countryRules"
          label="Country*"
          required
        ></v-text-field>
        
        <v-text-field
          v-model="City"
          :rules="nameRules"
          label="City*"
          required
        ></v-text-field>
        
        <v-text-field
          v-model="PostalCode"
          :rules="nameRules"
          label="Postal code*"
          required
        ></v-text-field>
        
        <v-text-field
          v-model="PhoneNumber"
          :rules="nameRules"
          label="Phone number"
          required
        ></v-text-field>
        
        
        <v-text-field
          v-model="email"
          :rules="emailRules"
          label="E-mail*"
          required
        ></v-text-field>

      <v-text-field
          v-model="password"
          :rules="emailRules"
          label="Password*"
          required
        ></v-text-field>

        <v-text-field
          v-model="Password"
          :rules="emailRules"
          label="Confirm Password*"
          required
        ></v-text-field>
          <v-spacer></v-spacer>
          <v-row justify="center">
              <h2 class="text-align">Your education</h2>
          </v-row>
          
        <v-select
          v-model="select"
          :levelStudies="levelStudies"
          :rules="[v => !!v || 'Item is required']"
          label="Level of studies*"
          required
        ></v-select>

        <v-select
          v-model="select"
          :groupOfschools="groupOfschools"
          :rules="[v => !!v || 'Item is required']"
          label="Group of schools*"
          required
        ></v-select>

          <v-combobox
        v-model="model"
        :items="items"
        :search-input.sync="search"
        hide-selected
        hint="Maximum of 3 Specializations"
        label="Add your Specialization"
        multiple
        persistent-hint
        small-chips
      >
        <template v-slot:no-data>
          <v-list-item>
            <v-list-item-content>
              <v-list-item-title>
                No results matching "<strong>{{ search }}</strong>". Press <kbd>enter</kbd> to create a new one
              </v-list-item-title>
            </v-list-item-content>
          </v-list-item>
        </template>
      </v-combobox>


        <br/>


        <v-checkbox
          v-model="checkbox"
          :rules="[v => !!v || 'You must agree to continue!']"
          label="Do you agree to our terms & conditions ?"
          required
        ></v-checkbox>


<v-btn
        :disabled="dialog"
        :loading="dialog"
        class="white--text"
        color="blue darken-2"
        @click="dialog = true"
      >
        Create Account
      </v-btn>
      <v-dialog
        v-model="dialog"
        hide-overlay
        persistent
        width="300"
      >
        <v-card
          color="blue"
          dark
        >
          <v-card-text>
            Please stand by
            <v-progress-linear
              indeterminate
              color="white"
              class="mb-0"
            ></v-progress-linear>
          </v-card-text>
        </v-card>
      </v-dialog>

      </v-form>

    


    </v-row> 
</v-container>

</template>
<script>
export default {
  name: 'Login',
  
  data: () => ({
dialog: false,
  valid: true,
    name: '',
    nameRules: [
      v => !!v || 'Name is required',
      v => (v && v.length <= 10) || 'Name must be less than 10 characters',
    ],
      
      
      loader: null,
      loading: false,
      loading2: false,
      loading3: false,
      loading4: false,
      loading5: false,
    
}),

watch: {
    loader () {
      const l = this.loader
      this[l] = !this[l]

      setTimeout(() => (this[l] = false), 3000)

      this.loader = null
    },
    dialog (val) {
      if (!val) return

      setTimeout(() => (this.dialog = false), 4000)
    },
},
 methods: {
    validate () {
      this.$refs.form.validate()
    },
 }
};
</script>