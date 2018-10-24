<template>
  <v-app>
    <v-navigation-drawer v-model="sidebar" app>
      <v-list>
        <v-list-tile v-for="item in menuItems" :key="item.title" @click="onNavigation(item.path)">
          <v-list-tile-action>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>{{ item.title }}</v-list-tile-content>
        </v-list-tile>
      </v-list>
    </v-navigation-drawer>
    <v-toolbar app :flat="!colored" dark :color="toolbarColor">
      <span class="hidden-sm-and-up">
        <v-toolbar-side-icon @click="sidebar = !sidebar">
        </v-toolbar-side-icon>
      </span>
      <v-btn icon @click.stop="clipped = !clipped">
        <img src="logo_light.png" alt="jkcit logo" height="35">
      </v-btn>
      <v-toolbar-title>
        <router-link to="/" tag="span" style="cursor: pointer">
          {{ title }}
        </router-link>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items class="hidden-xs-only">
        <v-btn flat v-for="item in menuItems" :key="item.title" @click="onNavigation(item.path)">
          <v-icon left dark>{{ item.icon }}</v-icon>
          {{ item.title }}
        </v-btn>
      </v-toolbar-items>
    </v-toolbar>
    <v-content class="pa-0" v-scroll="onScroll">
      <nuxt />
    </v-content>
    <v-footer height="auto" color="primary lighten-1">
      <v-layout justify-center row wrap>
        <v-btn v-for="link in links" :key="link" color="white" flat round @click="onNavigation(link.path)">
          {{ link.title }}
        </v-btn>
        <v-flex primary lighten-2 py-3 text-xs-center white--text xs12>
          &copy;2018 — <strong>{{title}}</strong>
        </v-flex>
      </v-layout>
    </v-footer>
  </v-app>
</template>

<script>
  export default {
    data() {
      return {
        sidebar: false,
        colored: false,
        menuItems: [
          { title: 'Home', path: '#home', icon: 'home' },
          { title: 'Services', path: '#services', icon: 'language' },
          { title: 'Courses', path: '#courses', icon: 'code' },
          { title: 'Contact Us', path: '#contact', icon: 'person' }
        ],
        links: [
          { title: 'Home', path: '#home', icon: 'home' },
          { title: 'Services', path: '#services', icon: 'language' },
          { title: 'Courses', path: '#courses', icon: 'code' },
          { title: 'Contact Us', path: '#contact', icon: 'person' }
        ],
        title: 'JKCIT Solutions'
      }
    },
    computed: {
      toolbarColor: function () {
        return this.colored ? 'primary' : 'transparent'
      }
    },
    methods: {
      onNavigation(section){
        this.$vuetify.goTo(section)
      },
      onScroll (e) {
        this.colored = window.scrollY > 100
      }
    }
  }

</script>
