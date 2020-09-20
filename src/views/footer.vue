<v-footer
        color="transparent"
        
      >
        <v-row>
          <v-spacer/> 
          <v-col md="3">
            <v-card
              max-width="200"
              flat
              app
            >
              <v-img
                max-width="190"
                src="../assets/logoBar.png"
              >
              </v-img>

              <v-card-text class="text--primary">
                <div>
                  <facebook-icon size="1.5x" class="custom-class icons"></facebook-icon>
                  <twitter-icon size="1.5x" class="custom-class icons"></twitter-icon>
                  <instagram-icon size="1.5x" class="custom-class icons"></instagram-icon>
                  <linkedin-icon size="1.5x" class="custom-class"></linkedin-icon>
                </div>
                
              </v-card-text>

              <v-card-text class="text--primary text-footer">
                <div  class="text-footer">
                © 2019. All rights reserved.
                </div>      
              </v-card-text>

            </v-card>
          </v-col>
          <v-col md="3">
            <v-card
              class="mx-auto"
              max-width="250"
              flat
              app
            >
              <v-card-text>
                <h2 class="display-1 text--primary">
                  Endereço
                </h2>
                <p style="font-size: 12px;line-height:2">
                  4077  Cabell Avenue Washington<br>
                  Virginia 20008 <br>
                  United States <br>
                  Phone: 703-564-3737
                </p>
              </v-card-text>
            </v-card>
          </v-col>
          <v-col md="3">
            <v-card
              class="mx-auto"
              max-width="200"
              flat
              app
            >
              <v-card-text>
                <h2 class="text--primary" style="margin-bottom:10px;">
                  Quick Links
                </h2>
                <a href="#" class="links-footer">Home</a> <br>
                <a href="#" class="links-footer">Como Usar</a> <br>
                <a href="#" class="links-footer">Serviços</a> <br>
                <a href="#" class="links-footer">FAQ</a> <br>
                <a href="#" class="links-footer">Contato</a> <br>

              </v-card-text>
              
            </v-card>

            
          </v-col>
          <v-spacer/>
        </v-row>
      </v-footer>




// script
import { FacebookIcon, TwitterIcon, InstagramIcon, LinkedinIcon } from 'vue-feather-icons'

components: {
    FacebookIcon, 
    TwitterIcon,
    InstagramIcon,
    LinkedinIcon
  },

// css

.icons{
  margin-top: 22px;
  margin-right: 25px;
}

.footer-card{
  margin-left: 20%;
  margin-bottom: 100px;
}
.text-footer{
  font-size: 12px;
}
.links-footer{
  text-decoration: none;
  margin-top: 20px;
  color: #3f3f3f;
}
