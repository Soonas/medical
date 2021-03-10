<template>
  <v-app :style="{ background: $vuetify.theme.themes.light.background }">
    <v-layout row>
      <v-flex md3>
        <v-app :style="{ background: $vuetify.theme.themes.light.background }">
          <v-container>
            <v-flex>
              <v-card class="ma-5 text-center mt-10" shaped elevation="10">

                <v-avatar class="mt-n7" size="60" elevation="10">
                  <img src="../assets/coco.png">
                </v-avatar>

                <v-card-title class="layout justify-center"
                  >Luana Maria</v-card-title
                >
                <v-card-subtitle class="layout justify-center"
                  >22 anos, Brasil</v-card-subtitle
                >

                <v-list-item>
                  <v-list-item-title class="cyan--text text--darken-1"
                    >Sangue</v-list-item-title
                  >
                  <v-list-item-title class="cyan--text text--darken-1"
                    >Altura</v-list-item-title
                  >
                  <v-list-item-title class="cyan--text text--darken-1"
                    >Peso</v-list-item-title
                  >
                </v-list-item>

                <v-list-item>
                  <v-list-item-subtitle>A+</v-list-item-subtitle>
                  <v-list-item-subtitle>165 cm</v-list-item-subtitle>
                  <v-list-item-subtitle>55 Kg</v-list-item-subtitle>
                </v-list-item>

              </v-card>
            </v-flex>

            <v-flex>
              <v-card class="ma-5 mt-n2" shaped elevation="10">
                <v-list>

                  <v-list-item>
                    <v-list-item-avatar size="10" color="cyan darken-1"></v-list-item-avatar>
                    <v-list-item-title class="ml-n2">Kognum</v-list-item-title>
                    <v-list-item-subtitle>10 mg</v-list-item-subtitle>
                  </v-list-item>

                  <v-list-item>
                    <v-list-item-title class="cyan--text text--darken-1">Seg</v-list-item-title>
                    <v-list-item-title class="cyan--text text--darken-1">Ter</v-list-item-title>
                    <v-list-item-title class="cyan--text text--darken-1">Qua</v-list-item-title>
                    <v-list-item-title class="cyan--text text--darken-1">Qui</v-list-item-title>
                  </v-list-item>

                  <v-list-item class="mt-n5">
                    <v-list-item-subtitle>2 vezes ao dia dia apos comer</v-list-item-subtitle>
                  </v-list-item>
                  <v-divider></v-divider>

                </v-list>

                <v-list two-line="" subheader="">
                  <v-list-item>
                    <v-list-item-avatar size="35">
                      <img src="../assets/coco2.jpg">
                    </v-list-item-avatar>

                    <v-list-item-content class="ml-n2">
                      <v-list-item-title>Dr. Marcia E. De Angeli</v-list-item-title>
                      <v-list-item-subtitle>Clinica de Ginicologia</v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-list>

                <v-list two-line="" subheader="" class="mt-5">
                  <v-list-item>
                    <v-list-item-title>Ginicologista</v-list-item-title>
                    <v-list-item-subtitle>hormonios femininos</v-list-item-subtitle>
                  </v-list-item>
                </v-list>

                <v-list two-line="" subheader="" class="my-n8">
                  <v-list-item>
                    <v-list-item-title class="cyan--text text--darken-1">Date</v-list-item-title>
                    <v-list-item-title class="cyan--text text--darken-1">Time</v-list-item-title>
                  </v-list-item>

                  <v-list-item class="mt-n10">
                    <v-list-item-title>10 Mar 2021</v-list-item-title>
                    <v-list-item-title >11:00</v-list-item-title>
                  </v-list-item>
                </v-list>
              </v-card>
            </v-flex>

            <v-flex>
              <v-card class="ma-5 text-center mt-6" shaped=" " elevation="10">
                
                <v-list-item three-line="">
                  <v-list-item-content>
                    <v-list-item-title class="headline mb-1">
                      <v-icon>fab fa-cc-visa</v-icon>
                    </v-list-item-title>
                    <v-list-item-subtitle>2345 4567 7889 5432</v-list-item-subtitle>
                  </v-list-item-content>

                  <v-list-item-avatar size="60" color="cyan darken-1">
                    <v-icon color="white">fas fa-plus</v-icon>
                  </v-list-item-avatar>
                </v-list-item>
                <!-- Card esta grudado, antes de prosseguir arrumar -->
              </v-card>
            </v-flex>
          </v-container>
        </v-app>
      </v-flex>
    </v-layout>
  </v-app>
</template>

<script>
// @ is an alias to /src
const gradients = [
  ["#222"],
  ["#42b3f4"],
  ["red", "orange", "yelllow"],
  ["purple", "violet"],
  ["#00c6ff", "#F0F", "#FF0"],
  ["#f72047", "#ffd200", "#1feaea"],
];

export default {
  data: () => ({
    with: 2,
    radius: 10,
    padding: 8,
    linecap: "round",
    gradient: gradients[5],
    value: [0, 2, 5, 9, 5, 10, 3, 5, 0, 0, 1, 8, 2, 9, 0],
    gradientDirection: "top",
    gradients,
    fill: false,
    type: "trend",
    autoLineWidth: false,
    arrayEvents: null,
    date2: new Date().toISOString().substr(0, 10),
  }),
  computed: {
    theme() {
      return this.$vuetify.theme.dark ? "dark" : "light";
    },
  },
  mounted() {
    this.arrayEvents = [...Array(6)].map(() => {
      const day = Math.floor(Math.random() * 30);
      const d = new Date();
      d.setDate(day);
      return d.toISOString().substr(0, 10);
    });
  },
  methods: {
    functionEvents(date) {
      const [, , day] = date.split("");
      if ([12, 17, 28].includes(parseInt(day, 10))) return true;
      if ([1, 19, 22].includes(parseInt(day, 10))) return ["red", "#00f"];
      return false;
    },
  },
};
</script>

<style scoped>
.rounded {
  border-top-left-radius: 50px;
  border-bottom-left-radius: 50px;
}
</style>