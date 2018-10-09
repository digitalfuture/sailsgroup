<template>
  <v-app dark>
    <v-content>
      <div class="price">
        <a href="/files/Sails Co Coffee Price.pdf" target="_blank">
          OPEN PRICE LIST
        </a>
      </div>
    </v-content>
    <v-footer fixed app class="grey--text transparent" height="auto">
      <v-layout column>
        <v-flex mb-5>
          <Contacts/>
        </v-flex>
        <p class="ml-3">&copy; {{ currentYear }} Sails Co</p>
      </v-layout>
    </v-footer>
  </v-app>
</template>

<script>
import Contacts from './components/Contacts'

export default {
  name: 'App',
  components: {
    Contacts
  },
  data() {
    return {}
  },
  computed: {
    currentYear: () => new Date().getFullYear()
  }
}
</script>
<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css?family=Barlow+Semi+Condensed');
#app {
  font-family: 'Barlow Semi Condensed', sans-serif;
  background: #212121 url('./assets/background.png') no-repeat right 0% top 0% /40%;

  .silver {
    color: silver;
  }

  a {
    color: lightgrey;
    text-decoration: none;

    &:hover {
      color: white;
    }
  }

  .price {
    margin: 40px;
  }
}
</style>
