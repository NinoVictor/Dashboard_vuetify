<template>
  <v-app>
    <NavigationDrawer></NavigationDrawer>
    <HeaderMain></HeaderMain>
    <v-main>
      <router-view></router-view>
    </v-main>
  </v-app>
</template>

<script>
import NavigationDrawer from "../components/NavigationDrawer";
import HeaderMain from "../components/HeaderMain";

export default {
  name: "Home",
  components: {
    NavigationDrawer,
    HeaderMain,
  },
};
</script>
