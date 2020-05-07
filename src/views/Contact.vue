<template>
  <div class="contact">
      <p> If you enjoy my work then feel free to contact me here. And i will reach out to you as soon as possible.</p>
  
  <v-form v-model="valid">
    <v-container>
      <v-row>
        <v-col
          cols="12"
          md="12"
        >
          <v-text-field
            v-model="name"
            :rules="nameRules"
            label="Name"
            required
          ></v-text-field>
        </v-col>

        <v-col
          cols="12"
          md="12"
        >
          <v-text-field
            v-model="email"
            :rules="emailRules"
            label="E-mail"
            required
          ></v-text-field>
        </v-col>

        <v-col
          cols="12"
          md="12"
        >
          <v-text-field
            v-model="message"
            :rules="messageRules"
            :counter="100"
            label="Message"
            required
          ></v-text-field>
        </v-col>
      </v-row>

    <v-btn class="mr-4" @click="send">send</v-btn>
    <v-btn @click="clear">clear</v-btn>

    </v-container>
  </v-form>


    </div>
  
</template>

<style scoped>
  p {
    text-align: center;
    margin-top: 50px;
  }
</style>


<script>
  export default {
    data: () => ({
      valid: false,
      name: '',
      nameRules: [
        v => !!v || 'Name is required',
        v => v.length <= 30 || 'Name must be less than 30 characters',
      ],
      email: '',
      emailRules: [
        v => !!v || 'E-mail is required',
        v => /.+@.+/.test(v) || 'E-mail must be valid',
      ],

      message: '',
      messageRules: [
        v => !!v || 'Message is required',
        v => v.length <= 100 || 'Message must be less than 100 characters',
      ],

    }),

    methods: {
      send () {
        this.$refs.observer.validate()
      },
      clear () {
        this.name = ''
        this.email = ''
        this.message = ''
        this.$refs.observer.reset()
      },
    },
  }
</script>


