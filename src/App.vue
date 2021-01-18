<template>
  <v-app>
    <v-main class="main">
      <div class="content text-center mx-auto w-5">
        <hr class="my-10 divider" />
        <h4 class="text-h1">
          Curtis <span class="font-weight-black">Haynes</span>
        </h4>
        <h5 class="text-h5 font-weight-light">Software Engineer</h5>
        <hr class="my-10 divider" />
        <div class="icon-container">
          <v-tooltip bottom>
            <template v-slot:activator="{ on, attrs }">
              <v-btn icon href="CCHaynes1122@gmail.com">
                <v-icon x-large color="white" v-bind="attrs" v-on="on"
                  >mdi-email</v-icon
                >
              </v-btn>
            </template>
            <span>Email</span>
          </v-tooltip>

          <v-tooltip bottom>
            <template v-slot:activator="{ on, attrs }">
              <v-btn icon href="https://github.com/CCHaynes112">
                <v-icon x-large color="white" v-bind="attrs" v-on="on"
                  >mdi-github</v-icon
                >
              </v-btn>
            </template>
            <span>Github</span>
          </v-tooltip>

          <v-tooltip bottom>
            <template v-slot:activator="{ on, attrs }">
              <v-btn
                icon
                href="https://www.linkedin.com/in/curtis-haynes-b608b015b/"
              >
                <v-icon x-large color="white" v-bind="attrs" v-on="on"
                  >mdi-linkedin</v-icon
                >
              </v-btn>
            </template>
            <span>LinkedIn</span>
          </v-tooltip>

          <v-tooltip bottom>
            <template v-slot:activator="{ on, attrs }">
              <v-btn icon href="http://google.com">
                <v-icon x-large color="white" v-bind="attrs" v-on="on"
                  >mdi-file-document</v-icon
                >
              </v-btn>
            </template>
            <span>Resume</span>
          </v-tooltip>
        </div>
      </div>
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: "App",

  components: {},

  data: () => ({
    //
  }),
};
</script>

<style scoped>
.main {
  /* background: #fafafa; */
  background-image: url("./assets/road-blur.jpg");
  background-size: cover; /* <------ */
  background-repeat: no-repeat;
  background-position: center center;
}
.content {
  color: white;
}
.divider {
  border: none;
  border-top: 1px groove white;
}
.icon-container {
  display: inline-flex;
  width: 200px;
  justify-content: space-between;
}
</style>