<template>
  <v-container>
    <v-row align="center" justify="center" style="height: 100vh;">
      <v-spacer />
      <v-col md="3" style="margin-top: 15%">
        <div class="paragraph">
          <h1>SERVIÇOS</h1>
          <p>Estes são alguns dos serviços oferecidos pela Juris.</p>
          <a>Saiba mais</a>
          <arrow-right-icon size="1x" style="margin-left: 10px; color: #1186B0;"></arrow-right-icon>
        </div>
      </v-col>
      <v-col md="6" style="margin-top: 25%;">
        <v-row no-gutters>
          <v-col cols="6">
            <v-card class="card" outlined>
              <v-row>
                <div class="divIcons">
                  <calendar-icon size="3x" class="icons"></calendar-icon>
                </div>
                <div class="divTexts">
                  <v-card-title style="color: black;">Agenda Personalizada</v-card-title>
                  <v-card-subtitle style="color: black;">
                    Crie sua própria agenda, com seus horários e gerencie
                    eles.
                  </v-card-subtitle>
                </div>
              </v-row>
            </v-card>
          </v-col>
          <v-col cols="6">
            <v-card class="card" color="transparent" outlined>
              <v-row>
                <div class="divIcons">
                  <clock-icon size="3x" class="icons"></clock-icon>
                </div>
                <div class="divTexts">
                  <v-card-title>Disponibilidade</v-card-title>
                  <v-card-subtitle style="color: white;">
                    Seus clientes podem ter acesso as
                    informações de qualquer lugar,
                    a qualquer hora de forma simples.
                  </v-card-subtitle>
                </div>
              </v-row>
            </v-card>
          </v-col>
          <v-col cols="6">
            <v-card class="card" color="transparent" outlined>
              <v-row>
                <div class="divIcons">
                  <shield-icon size="3x" class="icons"></shield-icon>
                </div>
                <div class="divTexts">
                  <v-card-title>Segurança</v-card-title>
                  <v-card-subtitle style="color: white;">
                    Os dados do seus clientes com a
                    proteção da nova lei LGPD.
                  </v-card-subtitle>
                </div>
              </v-row>
            </v-card>
          </v-col>
          <v-col cols="6">
            <div class="borderCard">
              <v-card class="borderCard" color="transparent" outlined>
                <v-row>
                  <div class="divIcons">
                    <settings-icon size="3x" class="icons"></settings-icon>
                  </div>
                  <div class="divTexts">
                    <v-card-title>Assistente Virtual Jurídico</v-card-title>
                    <v-card-subtitle style="color: white;">
                      Você terá um assistente que atende a
                      suas nescessidades, e que se adequa
                      a você.
                    </v-card-subtitle>
                  </div>
                </v-row>
              </v-card>
            </div>
          </v-col>
        </v-row>
      </v-col>
      <v-spacer />
    </v-row>
  </v-container>
</template>
<script>
import {
  ArrowRightIcon,
  CalendarIcon,
  ClockIcon,
  ShieldIcon,
  SettingsIcon,
} from "vue-feather-icons"

export default {
  components: {
    ArrowRightIcon,
    CalendarIcon,
    ClockIcon,
    ShieldIcon,
    SettingsIcon,
  },
}
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
.card {
  border-radius: 0 !important;
  margin: 0;
  height: 100%;
}
.icons {
  stroke-width: 0.5px;
  color: #1186b0;
}
div.v-card__title {
  font-size: 14px !important;
  color: white;
  font-weight: 300;
}
div.v-card__subtitle {
  font-size: 10px !important;
  font-weight: 100;
}
.divIcons {
  background-color: transparent;
  width: 25%;
  align-items: center;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: center;
}
.divTexts {
  width: 75%;
}
.borderCard {
  border-radius: 0 !important;
  margin: 0;
  height: 100%;
  border-top: 0.5px solid white !important;
  border-left: 0.5px solid white !important;
}
</style>
