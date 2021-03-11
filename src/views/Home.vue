<template>
  <v-app :style="{ background: $vuetify.theme.themes.light.background }">
    <v-layout row>
      <v-flex md3>
        <v-app :style="{ background: $vuetify.theme.themes.light.background }">
          <v-container>
            <v-flex>
              <v-card class="ma-5 text-center mt-12" shaped elevation="10">
                <v-avatar class="mt-n7" size="60" elevation="10">
                  <img src="../assets/coco.png"/>
                </v-avatar>
                <v-card-title class="layout justify-center"
                  >Luana Maria</v-card-title
                >
                <v-card-subtitle class="layout justify-center"
                  >21 anos, Brasil</v-card-subtitle
                >
                <v-list>
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
                  <v-list-item class="mt-n5">
                    <v-list-item-subtitle>A+</v-list-item-subtitle>
                    <v-list-item-subtitle>165 cm</v-list-item-subtitle>
                    <v-list-item-subtitle>55 Kg</v-list-item-subtitle>
                  </v-list-item>
                </v-list>
              </v-card>
            </v-flex>
            <v-flex>
              <v-list color="transparent" class="text-center">
                <v-list-item>
                  <v-list-item-title class="cyan--text text--darken-1"
                    >Notificações</v-list-item-title
                  >
                  <v-list-item-subtitle>10 Mar 2021</v-list-item-subtitle>
                </v-list-item>
              </v-list>
            </v-flex>
            <v-flex>
              <v-card class="ma-5" shaped elevation="10">
                <v-list>
                  <v-list-item>
                    <v-list-item-avatar
                      size="10"
                      color="cyan darken-1"
                    ></v-list-item-avatar>
                    <v-list-item-title class="ml-n2">Glicose</v-list-item-title>
                    <v-list-item-subtitle>10 mg</v-list-item-subtitle>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-title class="cyan--text text--darken-1"
                      >Seg</v-list-item-title
                    >
                    <v-list-item-title class="cyan--text text--darken-1"
                      >Ter</v-list-item-title
                    >
                    <v-list-item-title class="cyan--text text--darken-1"
                      >Qua</v-list-item-title
                    >
                    <v-list-item-title class="cyan--text text--darken-1"
                      >Qui</v-list-item-title
                    >
                  </v-list-item>
                  <v-list-item class="mt-n5">
                    <v-list-item-subtitle
                      >2 vezes ao dia depois de comer</v-list-item-subtitle
                    >
                  </v-list-item>
                  <v-divider></v-divider>
                </v-list>
                <v-list two-line subheader>
                  <v-list-item>
                    <v-list-item-avatar size="35">
                      <img src="../assets/coco2.jpg"/>
                    </v-list-item-avatar>
                    <v-list-item-content class="ml-n2">
                      <v-list-item-title
                        >Dra. Marcia E. De Angeli</v-list-item-title
                      >
                      <v-list-item-subtitle
                        >Clinica De Angeli</v-list-item-subtitle
                      >
                    </v-list-item-content>
                  </v-list-item>
                </v-list>
                <v-list two-line subheader class="mt-n5">
                  <v-list-item>
                    <v-list-item-content>
                      <v-list-item-title>Ginicologista</v-list-item-title>
                      <v-list-item-subtitle>Dor no útero</v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-list>
                <v-list two-line subheader class="mt-n8">
                  <v-list-item>
                    <v-list-item-title class="cyan--text text--darken-1"
                      >Data</v-list-item-title
                    >
                    <v-list-item-title class="cyan--text text--darken-1"
                      >Horas</v-list-item-title
                    >
                  </v-list-item>
                  <v-list-item class="mt-n10">
                    <v-list-item-title>10 Mar 2021</v-list-item-title>
                    <v-list-item-title>21:24</v-list-item-title>
                  </v-list-item>
                </v-list>
              </v-card>
            </v-flex>
            <v-flex>
              <v-card class="ma-5 text-center mt-12" shaped elevation="10">
                <v-list-item three-line>
                  <v-list-item-content>
                    <v-list-item-title class="headline mb-1">
                      <v-icon>fab fa-cc-visa</v-icon>
                    </v-list-item-title>
                    <v-list-item-subtitle
                      >2345 4645 7865 5432</v-list-item-subtitle
                    >
                  </v-list-item-content>

                  <v-list-item-avatar size="60" color="cyan darken-1">
                    <v-icon color="white">fas fa-plus</v-icon>
                  </v-list-item-avatar>
                </v-list-item>
              </v-card>
            </v-flex>
          </v-container>
        </v-app>
      </v-flex>
      <v-flex md9>
        <v-app
          :style="{ background: $vuetify.theme.themes.dark.background }"
          class="rounded"
        >
          <v-container>
            <v-flex>
              <v-list class="mt-5">
                <v-list-item>
                  <v-list-item-title class="cyan--text text--darken-1"
                    >Examinação</v-list-item-title
                  >
                  <v-list-item-action>
                    <v-btn class="ma-2" tile outlined color="cyan darken-1">
                      <v-icon left>fas fa-eye</v-icon>See All
                    </v-btn>
                  </v-list-item-action>
                </v-list-item>
              </v-list>
            </v-flex>
            <v-flex>
              <v-row no-gutters>
                <v-col cols="12" md="4">
                  <v-row>
                    <v-col cols="12" md="2">
                      <v-card height="80px" width="10px" color="green"></v-card>
                    </v-col>
                    <v-col cols="12" md="10">
                      <v-list two-line subheader class="ml-n8">
                        <v-list-item>
                          <v-list-item-content>
                            <v-list-item-subtitle
                              >21 Jul, 2019</v-list-item-subtitle
                            >
                            <v-list-item-title
                              >Crises de Hipertensão</v-list-item-title
                            >
                            <v-list-item-subtitle
                              >Tratamento em Andamento</v-list-item-subtitle
                            >
                          </v-list-item-content>
                        </v-list-item>
                      </v-list>
                    </v-col>
                  </v-row>
                </v-col>
                <v-col cols="12" md="4">
                  <v-row>
                    <v-col cols="12" md="2">
                      <v-card height="80px" width="10px" color="red"></v-card>
                    </v-col>
                    <v-col cols="12" md="10">
                      <v-list two-line subheader class="ml-n8">
                        <v-list-item>
                          <v-list-item-content>
                            <v-list-item-subtitle
                              >18 Jul, 2020</v-list-item-subtitle
                            >
                            <v-list-item-title>Osteoporose</v-list-item-title>
                            <v-list-item-subtitle
                              >Incuravel</v-list-item-subtitle
                            >
                          </v-list-item-content>
                        </v-list-item>
                      </v-list>
                    </v-col>
                  </v-row>
                </v-col>
                <v-col cols="12" md="4">
                  <v-row>
                    <v-col cols="12" md="2">
                      <v-card height="80px" width="10px" color="grey"></v-card>
                    </v-col>
                    <v-col cols="12" md="10">
                      <v-list two-line subheader class="ml-n8">
                        <v-list-item>
                          <v-list-item-content>
                            <v-list-item-subtitle
                              >21 Jul, 2021</v-list-item-subtitle
                            >
                            <v-list-item-title
                              >Crises de Hipertensão</v-list-item-title
                            >
                            <v-list-item-subtitle
                              >Examinações</v-list-item-subtitle
                            >
                          </v-list-item-content>
                        </v-list-item>
                      </v-list>
                    </v-col>
                  </v-row>
                </v-col>
              </v-row>
            </v-flex>
            <v-flex>
              <v-list class="mt-5">
                <v-list-item>
                  <v-list-item-title class="cyan--text text--darken-1"
                    >Curva da Saúde</v-list-item-title
                  >
                  <v-item-content>
                    <v-btn class="mr-1" outlined color="cyan darken-1">Seg</v-btn>
                  </v-item-content>
                  <v-item-content>
                    <v-btn class="mr-1" outlined color="cyan darken-1">Ter</v-btn>
                  </v-item-content>
                  <v-item-content>
                    <v-btn class="mr-1" outlined color="cyan darken-1">Qua</v-btn>
                  </v-item-content>
                  <v-item-content>
                    <v-btn outlined color="cyan darken-1">Qui</v-btn>
                  </v-item-content>
                </v-list-item>
              </v-list>
            </v-flex>
            <v-flex>
              <v-sparkline
                :value="value"
                :gradient="gradient"
                :smooth="radius || false"
                :padding="padding"
                :line-width="width"
                :stroke-linecap="lineCap"
                :gradient-direction="gradientDirection"
                :fill="fill"
                :type="type"
                :auto-line-width="autoLineWidth"
                auto-draw
              ></v-sparkline>
            </v-flex>
            <v-flex class="mt-5">
              <v-list class="ml-5">
                <v-list-item>
                  <v-list-item-avatar
                    color="cyan darken-1"
                    size="20px"
                  ></v-list-item-avatar>
                  <v-list-item-title>Média</v-list-item-title>
                  <v-list-item-avatar
                    color="cyan darken-1"
                    size="20px"
                  ></v-list-item-avatar>
                  <v-list-item-title class="ml-5">Meus Dados</v-list-item-title>
                </v-list-item>
              </v-list>
            </v-flex>
            <v-flex>
              <v-list class="ml-5">
                <v-list-item>
                  <v-list-item-title class="cyan--text text--darken-1"
                    >Próximo Tratamento</v-list-item-title
                  >
                  <v-list-item-title class="cyan--text text--darken-1"
                    >Aviso</v-list-item-title
                  >
                </v-list-item>
              </v-list>
            </v-flex>
            <v-flex class="ml-8">
              <v-row>
                <div>
                  <v-date-picker
                    v-model="date2"
                    :event-color="(date) => (date[9] % 2 ? 'red' : 'yellow')"
                    :events="functionEvents"
                  ></v-date-picker>
                </div>
                <div class="ml-5">
                  <v-list>
                    <v-list-item>
                      <v-list-item-title
                        >O serviço Clínico é consultado e disponível 24 Horas</v-list-item-title>
                    </v-list-item>
                  </v-list>
                </div>
              </v-row>
            </v-flex>
          </v-container>
        </v-app>
      </v-flex>
    </v-layout>
  </v-app>
</template>
<script>
const gradients = [
  ["#222"],
  ["#42b3f4"],
  ["red", "orange", "yellow"],
  ["purple", "violet"],
  ["#00c6ff", "#F0F", "#FF0"],
  ["#f72047", "#ffd200", "#1feaea"],
];
export default {
  data: () => ({
    width: 2,
    radius: 10,
    padding: 8,
    lineCap: "round",
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
      const [, , day] = date.split("-");
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