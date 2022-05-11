<template>
    <v-app>
        <v-navigation-drawer app>
        </v-navigation-drawer>

        <v-app-bar app>
        </v-app-bar>
        <v-main>
            <v-container fluid>
                <HelloWorld msg="Tauri app with Vuetify"></HelloWorld>
                <v-btn elevation="2" rounded @click="test">Vuetify button {{ count }}</v-btn>
            </v-container>
        </v-main>

        <v-footer app>
        </v-footer>
    </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  },
  data() {
      return {
          count: 0
      }
  },
  methods: {
    test() {
        this.count = 5
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
