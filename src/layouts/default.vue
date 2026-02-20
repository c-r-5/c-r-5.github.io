<template>
  <v-app>
    <!-- Navigation Drawer for mobile -->
    <v-navigation-drawer
      v-model="drawer"
      temporary
      v-if="!smAndUp"
    >
      <v-list>
        <v-list-item link to="/">
          <v-list-item-title>Home</v-list-item-title>
        </v-list-item>
        <v-list-item link to="/about">
          <v-list-item-title>About</v-list-item-title>
        </v-list-item>
        <v-list-item link to="/projects">
          <v-list-item-title>Projects</v-list-item-title>
        </v-list-item>
        <v-list-item link to="/contact">
          <v-list-item-title>Contact</v-list-item-title>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>

    <v-app-bar app dense elevated>
      <v-container fluid class="px-4">
        <div class="d-flex align-center justify-space-between w-100">
          <div class="d-flex align-center pa-0">
            <v-app-bar-nav-icon v-if="!smAndUp" @click="drawer = !drawer" />

            <router-link to="/" custom v-slot="{ navigate, href, isActive }">
              <v-toolbar-title
                class="text-h6 ps-4"
                role="button"
                :aria-current="isActive ? 'page' : null"
                @click="navigate"
                :href="href"
              >
                しーある
              </v-toolbar-title>
            </router-link>
          </div>

          <div v-if="smAndUp" class="d-flex gap-3 align-center">
            <v-btn text to="/">Home</v-btn>
            <v-btn text to="/about">About</v-btn>
            <v-btn text to="/projects">Projects</v-btn>
            <v-btn text to="/contact">Contact</v-btn>
          </div>
        </div>
      </v-container>
    </v-app-bar>

    <v-main>
      <router-view />
    </v-main>

    <AppFooter />
  </v-app>
</template>

<script setup>
import { ref } from 'vue'
import { useDisplay } from 'vuetify'

const drawer = ref(false)
const { smAndUp } = useDisplay()
</script>
