<template>
  <v-app @click="handleOutsideClick">
    <!-- Navigation Drawer -->
    <v-navigation-drawer v-model="drawer" app width="240" clipped permanent>
      <v-list>
        <v-list-item>
          <v-list-item-title>Home</v-list-item-title>
        </v-list-item>
        <v-list-item>
          <v-list-item-title>About</v-list-item-title>
        </v-list-item>
        <v-list-item>
          <v-list-item-title>Contact</v-list-item-title>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>

    <!-- App Bar -->
    <v-app-bar app color="primary" dark elevate-on-scroll clipped-left>
      <v-app-bar-nav-icon
        class="btn"
        @click="toggleDrawer"
      ></v-app-bar-nav-icon>
      <v-toolbar-title>FOODIE</v-toolbar-title>
    </v-app-bar>

    <!-- Main Content -->
    <v-main>
      <v-container>
        <h1>Welcome to Foodie!</h1>
        <p>Explore our awesome menu and services.</p>
      </v-container>
    </v-main>
  </v-app>
</template>
  
  <script setup>
import { ref } from "vue";

// Drawer state
const drawer = ref(false); // Initially open

// Function to toggle the drawer
const toggleDrawer = () => {
  drawer.value = !drawer.value;
};

// Function to close the drawer if clicked outside of it
const handleOutsideClick = (e) => {
  // Check if the click target is outside the navigation drawer
  const drawerElement = document.querySelector(".v-navigation-drawer");
  const drawerElement2 = document.querySelector(".btn");
  if (
    drawer &&
    drawerElement &&
    !drawerElement.contains(e.target) &&
    drawerElement2 &&
    !drawerElement2.contains(e.target)
  ) {
    drawer.value = false;
  }
};
</script>
  
  <style scoped>
/* Adjusting the v-app-bar to move when the navigation drawer opens */
.v-navigation-drawer--clipped {
  transition: width 0.3s ease;
}

.v-app-bar {
  transition: margin-left 0.3s ease;
}
</style>
  