<template>
  <v-container fluid>
    <v-layout row justify-center align-center>
      <v-flex xs12 sm9 md6>
        <v-layout wrap row align-end>
          <v-flex xs12 sm3 md3 pl-3 pt-3>
            <img src="@/assets/logo.png" alt="Sails Co" class="logo" />
          </v-flex>
          <v-flex xs12 sm10 md9 pl-3 pt-3>
            <v-layout no-wrap>
              <div class="contacts">
                <span
                  >phone: &ensp;<span class="silver"
                    >+84 825 520 025 &nbsp;&nbsp;</span
                  >/ Vietnam</span
                ><br />
                <span
                  >email: &ensp;<a href="mailto:mail@sails-group.com"
                    >mail@sails-group.com</a
                  ></span
                >
              </div>
            </v-layout>
          </v-flex>
        </v-layout>
      </v-flex>
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
.contacts {
  font-size: 20px;
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
}

.logo {
  width: 110px;
  height: 110px;
  display: block;
}
</style>
