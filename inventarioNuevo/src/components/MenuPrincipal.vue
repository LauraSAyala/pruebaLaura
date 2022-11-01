<template>
  <v-card
    class="mx-auto overflow-hidden"
    height="400"
    
  >
    <v-app-bar
      color="accent"
      dark
    >
      <v-app-bar-nav-icon @click="drawer = true"></v-app-bar-nav-icon>

      <v-toolbar-title>Pateleria Salvato</v-toolbar-title>
    </v-app-bar>

    <v-navigation-drawer
      v-model="drawer"
      absolute
      temporary
    >
      <v-list
        nav
        dense
      >
        <v-list-item-group
          v-model="group"
          active-class="deep-purple--text text--accent-4"
        >
          <v-list-item :to="'/compras'">
            <v-list-item-icon>
              <v-icon>mdi-home</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Compra</v-list-item-title>
          </v-list-item>

          <v-list-item :to="'/ventas'">
            <v-list-item-icon>
              <v-icon>mdi-account</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Venta</v-list-item-title>
          </v-list-item>

          <!-- <v-list-item>
            <v-list-item-icon>
              <v-icon>mdi-nosotros</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Nosotros</v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-icon>
              <v-icon>mdi-contactenos</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Contactenos</v-list-item-title>
          </v-list-item> -->

        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
  </v-card>
</template>

<script>
  export default {
    data: () => ({
      drawer: false,
      group: null,
    }),
  }
</script>

<style>
</style>