<template>
  <v-app dark>
    <v-content>
      <Contacts/>
    </v-content>
    <v-footer fixed app class="grey--text">
      <span class="ml-3">&copy; {{ currentYear }} Sails Co</span>
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
  background: #212121;
}
</style>
