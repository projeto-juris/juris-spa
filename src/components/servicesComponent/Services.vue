<template>
  <v-container>
    <v-row align="center" justify="center" style="height: 100vh;">
      <v-spacer />
      <v-col md="3">
        <div class="paragraph">
          <h1>SERVIÇOS</h1>
          <p>Estes são alguns dos serviços oferecidos pela Juris.</p>
          <a>Saiba mais</a>
          <arrow-right-icon
            size="1x"
            style="margin-left: 10px; color: #1186B0;"
          ></arrow-right-icon>
        </div>
      </v-col>
      <v-col md="7">
        <v-row dense>
          <v-col cols="6">
            <v-card class="card">
              <v-row>
                <v-col md="3">
                  <div class="divIcons">
                    <calendar-icon size="5x" class="icons"></calendar-icon>
                  </div>
                </v-col>
                <v-col md="9">
                  <v-card-title>Agenda personalizada</v-card-title>
                  <v-card-subtitle
                    >Crie sua própria agenda, com seus horários e gerencie
                    eles.</v-card-subtitle
                  >
                </v-col>
              </v-row>
            </v-card>
          </v-col>
          <v-col cols="6">
            <v-card></v-card>
          </v-col>
        </v-row>
        <v-row dense>
          <v-col cols="6">
            <v-card></v-card>
          </v-col>
          <v-col cols="6">
            <v-card></v-card>
          </v-col>
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>
<script>
import { ArrowRightIcon } from "vue-feather-icons";
import { CalendarIcon } from "vue-feather-icons";

export default {
  components: {
    ArrowRightIcon,
    CalendarIcon,
  },
};
</script>
<style>
.paragraph > * {
  color: white;
  font-weight: 300;
}
.paragraph > h1 {
  letter-spacing: 3px;
}
.paragraph > a {
  text-decoration: none;
  color: white;
}
.icons {
  stroke-width: 0.8px;
  color: #1186b0;
}
.v-card__title {
  font-size: 15px;
}
.divIcons {
}
</style>
