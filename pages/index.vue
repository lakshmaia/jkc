<template>
  <v-layout>
    <v-flex xs12>
      <section id="home">
        <v-parallax src="dam.jpg" height="500">
          <v-layout column align-center justify-center class="white--text">
            <img src="logo.png" alt="jkcit logo" height="100">
            <h1 class="white--text mb-2 display-1 text-xs-center">JKCIT Solutions</h1>
            <div class="subheading mb-3 text-xs-center">Endless Development</div>
            <v-btn class="orange lighten-2 mt-5" dark large @click="$vuetify.goTo('#contact')">
              Contact US
            </v-btn>
          </v-layout>
        </v-parallax>
      </section>

      <section id="services">
        <v-layout column wrap class="my-5" align-center>
          <v-flex xs12 sm4 class="my-3">
            <div class="text-xs-center">
              <h2 class="headline">The best way to start developing a bright future</h2>
              <span class="subheading">
                
              </span>
            </div>
          </v-flex>
          <v-flex xs12>
            <v-container grid-list-xl>
              <v-layout row wrap align-center>
                <v-flex xs12 md4>
                  <v-card class="elevation-0 transparent">
                    <v-card-text class="text-xs-center">
                      <v-icon x-large color="primary">chat</v-icon>
                    </v-card-text>
                    <v-card-title primary-title class="layout justify-center">
                      <div class="headline text-xs-center">Development & Job Support</div>
                    </v-card-title>
                    <v-card-text>
                      We have an efficient IT team who help you in resolving the issues according to the technical protocols.
                    </v-card-text>
                  </v-card>
                </v-flex>
                <v-flex xs12 md4>
                  <v-card class="elevation-0 transparent">
                    <v-card-text class="text-xs-center">
                      <v-icon x-large color="primary">code</v-icon>
                    </v-card-text>
                    <v-card-title primary-title class="layout justify-center">
                      <div class="headline">Corportate Training</div>
                    </v-card-title>
                    <v-card-text>
                    We understand the complications involved in designing, developing and implementing the project. 
                    Thus, we help you in planning, organising, and controlling the resources to accomplish the specified 
                    goals( especially for startups).
                    </v-card-text>
                  </v-card>
                </v-flex>
                <v-flex xs12 md4>
                  <v-card class="elevation-0 transparent">
                    <v-card-text class="text-xs-center">
                      <v-icon x-large color="primary">language</v-icon>
                    </v-card-text>
                    <v-card-title primary-title class="layout justify-center">
                      <div class="headline text-xs-center">Learn courses online</div>
                    </v-card-title>
                    <v-card-text>
                      We will help you in giving tutorials(in telugu and english) which are quick and easy to understand 
                      languages such as Java, ORACLE ,HADOOP,SAP MODULES,Amazon Web Services etc 
                    </v-card-text>
                  </v-card>
                </v-flex>
              </v-layout>
            </v-container>
          </v-flex>
        </v-layout>
      </section>

      <section id="courses">
        <v-card class="pa-5" color="primary" flat>
          <v-container grid-list-xl>
            <v-layout row wrap justify-center class="my-5">
              <div class="text-xs-center">
                <v-chip color="secondary" text-color="white">Java</v-chip>
                <v-chip color="secondary" text-color="white">Data Science</v-chip>
                <v-chip color="secondary" text-color="white">Cloud Computing</v-chip>
                <v-chip color="secondary" text-color="white">Data Warehousing-Informatica</v-chip>
                <v-chip color="secondary" text-color="white">Qlikview</v-chip>
                <v-chip color="secondary" text-color="white">IBM Websphere</v-chip>
                <v-chip color="secondary" text-color="white">Big Data</v-chip>
                <v-chip color="secondary" text-color="white">Hadoop</v-chip>
                <v-chip color="secondary" text-color="white">DevOps</v-chip>
                <v-chip color="secondary" text-color="white">Angular</v-chip>
                <v-chip color="secondary" text-color="white">NodeJS</v-chip>
                <v-chip color="secondary" text-color="white">ETL</v-chip>
                <v-chip color="secondary" text-color="white">WebLogic</v-chip>
                <v-chip color="secondary" text-color="white">Python</v-chip>
                <v-chip color="secondary" text-color="white">C/C++</v-chip>
                <v-chip color="secondary" text-color="white">Tableau</v-chip>
                <v-chip color="secondary" text-color="white">SAP</v-chip>
                <v-chip color="secondary" text-color="white">PHP</v-chip>
                <v-chip color="secondary" text-color="white">MySQL</v-chip>
              </div>
            </v-layout>
          </v-container>
        </v-card>
      </section>

      <section>
        <v-parallax src="support.jpg" height="380">
          <v-layout column align-center justify-center>
            <div class="headline white--text mb-3 text-xs-center">Being a developer has never been easier</div>
            <em>Kick-start your career today</em>
            <v-btn class="blue lighten-2 mt-5" dark large @click="$vuetify.goTo('#contact')" >
              Get Started
            </v-btn>
          </v-layout>
        </v-parallax>
      </section>

      <section id="contact">
        <v-container grid-list-xl>
          <v-layout row wrap justify-center class="my-5">
            <v-flex xs12 sm4>
              <v-card class="elevation-0 transparent">
                <v-card-title primary-title class="layout justify-center">
                  <div class="headline">Company info</div>
                </v-card-title>
                <v-card-text>
            JKCIT Solutions is a Software Technology Training cum Development Company situated in Hyderabad. 
            It's management and teaching faculty includes either working IT professionals/expertise in IT industry. 
            The training is completely industry oriented and interview oriented. During the initial days of training itself, 
            All the concepts will be taught with realtime examples and in an easily understandable way. 
            Currently we operate as three strategic business units focusing on IT Training, IT Services and IT Staffing.
                </v-card-text>
              </v-card>
            </v-flex>
            <v-flex xs12 sm4 offset-sm1>
              <v-card class="elevation-0 transparent">
                <v-card-title primary-title class="layout justify-center">
                  <div class="headline">Contact us</div>
                </v-card-title>
                <v-card-text>
                  If you want to avail our services, you can contact us
                </v-card-text>
                <v-list class="transparent">
                  <v-list-tile>
                    <v-list-tile-action>
                      <v-icon color="secondary">phone</v-icon>
                    </v-list-tile-action>
                    <v-list-tile-content>
                      <v-list-tile-content>+91 8074804038, +1 6038929631</v-list-tile-content>
                    </v-list-tile-content>
                  </v-list-tile>
                  <v-list-tile>
                    <v-list-tile-action>
                      <v-icon color="secondary">place</v-icon>
                    </v-list-tile-action>
                    <v-list-tile-content>
                      <v-list-tile-content>#827, Sanvi Residency, KPBH, Hyderabad, India</v-list-tile-content>
                    </v-list-tile-content>
                  </v-list-tile>
                  <v-list-tile>
                    <v-list-tile-action>
                      <v-icon color="secondary">email</v-icon>
                    </v-list-tile-action>
                    <v-list-tile-content>
                      <v-list-tile-title>jkcitsolutions@gmail.com</v-list-tile-title>
                    </v-list-tile-content>
                  </v-list-tile>
                </v-list>
              </v-card>
            </v-flex>
          </v-layout>
        </v-container>
      </section>
    </v-flex>
  </v-layout>
</template>

<script>

  export default {

  }

</script>
