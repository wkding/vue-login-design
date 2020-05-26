<template>

  <v-app>
    <v-app-bar
      app
      color="black"
      dark
    >
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-logo-dark.png"
          transition="scale-transition"
          width="40"
        />

        <v-app-toolbar>Login App</v-app-toolbar>
      </div>

      <v-spacer></v-spacer>

      <v-btn
        href="https://github.com/Nayalash/login-design-vue"
        target="_blank"
        text
      >
        <span class="mr-2">Home</span>
        <v-icon>mdi-Github</v-icon>
      </v-btn>
    </v-app-bar>


    <v-content>
      <v-container
              class="fill-height"
              fluid
      >
        <v-row
                align="center"
                justify="center"
        >
          <v-col
                  cols="12"
                  sm="8"
                  md="4"
          >
            <v-card class="elevation-12">
              <v-toolbar
                      color="black"
                      dark
                      flat
              >
                <v-toolbar-title>Login</v-toolbar-title>

              </v-toolbar>

              <v-card-text>
                <v-form>
                  <v-text-field
                          label="Login"
                          name="login"
                          prepend-icon="@:"
                          type="text"
                  ></v-text-field>

                  <v-text-field
                          id="password"
                          label="Password"
                          name="password"
                          prepend-icon="P:"
                          type="password"
                  ></v-text-field>
                </v-form>
              </v-card-text>
              <v-card-actions>
                <v-spacer></v-spacer>
                <v-btn color="grey">Login</v-btn>
              </v-card-actions>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-content>

  </v-app>
</template>

<script>
export default {
  name: 'App',
  props: {
    source: String,
  },
  data: () => ({
    //
  }),
};
</script>
