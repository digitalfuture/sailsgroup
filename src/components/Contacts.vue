<template>
  <v-container fluid class="full-height">
    <v-layout column align-center class="full-height">
      <v-layout row align-center>
        <v-layout row wrap>
          <v-flex xs12 sm6>
            <img src="@/assets/logo.png" alt="Sails Co" class="mb-5 logo">
          </v-flex>
          <v-flex xs12 sm6 no-wrap class="contacts">
            <br>
            <br>
            <span>phone: +84 129 55 20 025  &nbsp;&nbsp;/ Vietnam</span>
            <p>email: <a href="mailto:mail@sailsgroup@online">mail@sailsgroup.online</a></p>
          </v-flex> 
        </v-layout>
      </v-layout>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  name: 'Contacts'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
.full-height {
  height: 100%;
}
.contacts {
  a {
    color: silver;
    text-decoration: none;
    &:hover {
      color: lightgrey;
    }
  }
  color: silver;
  font-size: 20px;
}
.logo {
  width: 120px;
}
</style>
