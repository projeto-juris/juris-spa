<template>
  <v-footer color="transparent">
    <v-row>
      <v-spacer />
      <v-col md="1.5">
        <v-card max-width="200" flat color="transparent" app>
          <v-card-actions>
            <v-img max-width="190" src="../assets/logoBar.png"></v-img>
          </v-card-actions>
          <v-card-text class="text--primary">
            <div>
              <facebook-icon size="1.5x" class="footerIcons"></facebook-icon>
              <twitter-icon size="1.5x" class="footerIcons"></twitter-icon>
              <instagram-icon size="1.5x" class="footerIcons"></instagram-icon>
              <linkedin-icon size="1.5x" class="footerIcons" style="margin: 0;"></linkedin-icon>
            </div>
          </v-card-text>

          <v-card-text class="text--primary text-footer">
            <div class="text-footer">© 2019. All rights reserved.</div>
          </v-card-text>
        </v-card>
      </v-col>
      <v-col md="3">
        <v-card color="transparent " class="mx-auto" max-width="250" flat app>
          <v-card-text>
            <h2 class="display-1 text--primary">Endereço</h2>
            <p style="font-size: 12px;line-height:2">
              4077 Cabell Avenue Washington
              <br />Virginia 20008
              <br />United States
              <br />Phone: 703-564-3737
            </p>
          </v-card-text>
        </v-card>
      </v-col>
      <v-col md="2">
        <v-card color="transparent" class="mx-auto" max-width="200" flat app>
          <v-card-text>
            <h2 class="text--primary" style="margin-bottom:10px;">Quick Links</h2>
            <a href="#" class="linksFooter">Home</a>
            <br />
            <a href="#" class="linksFooter">Como Usar</a>
            <br />
            <a href="#" class="linksFooter">Serviços</a>
            <br />
            <a href="#" class="linksFooter">FAQ</a>
            <br />
            <a href="#" class="linksFooter">Contato</a>
            <br />
          </v-card-text>
        </v-card>
      </v-col>
      <v-spacer />
    </v-row>
  </v-footer>
</template>
<script>
import {
  FacebookIcon,
  TwitterIcon,
  InstagramIcon,
  LinkedinIcon,
} from "vue-feather-icons"
export default {
  components: {
    FacebookIcon,
    TwitterIcon,
    InstagramIcon,
    LinkedinIcon,
  },
}
</script>
<style>
.footerIcons {
  margin-top: 22px;
  margin-right: 25px;
  color: white;
  border: 0.5px solid white;
  border-radius: 10px;
  padding: 4px;
}

.footer-card {
  margin-left: 20%;
  margin-bottom: 100px;
}
.text-footer {
  color: white;
  font-size: 12px;
}
.linksFooter {
  text-decoration: none !important;
  color: #3f3f3f !important;
  margin-top: 20px;
}
</style>
