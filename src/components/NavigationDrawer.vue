<template>
  <v-navigation-drawer app permanent expand-on-hover class="pink">
    <v-list>
      <v-list-item v-for="item in items" :key="item.title" link>
        <v-list-item-icon>
          <v-icon class="white--text">{{ item.icon }}</v-icon>
        </v-list-item-icon>

        <v-list-item-content>
          <v-list-item-title class="white--text">{{
            item.title
          }}</v-list-item-title>
        </v-list-item-content>
      </v-list-item>
    </v-list>
    <v-divider></v-divider>
    <template v-slot:append>
      <div class="pa-2">
        <v-list-item link>
          <v-list-item-icon>
            <v-icon class="white--text">mdi-exit-to-app</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title class="white--text"
              >Cerrar sesión</v-list-item-title
            >
          </v-list-item-content>
        </v-list-item>
      </div>
    </template>
  </v-navigation-drawer>
</template>

<script>
export default {
  name: "NavigationDrawer",
  data: () => ({
    items: [
      { title: "Cobro", icon: "mdi-gavel" },
      { title: "Cursos", icon: "mdi-school" },
      { title: "Planteles", icon: "mdi-domain" },
    ],
  }),
};
</script>

<style></style>
