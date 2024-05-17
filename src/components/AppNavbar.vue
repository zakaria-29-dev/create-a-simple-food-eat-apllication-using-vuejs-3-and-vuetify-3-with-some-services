<template>
  <v-app-bar color="transparent" flat scroll-behavior="hide">
    <v-toolbar-title class="text-orange-darken-3">FOODEAT</v-toolbar-title>

    <v-spacer></v-spacer>

    <v-tabs bg-color="transparent" color="#9B7150" fixed-tabs>
      <v-tab text="HOME"></v-tab>
      <v-tab text="MENU"></v-tab>
      <v-tab text="ABOUT"></v-tab>
    </v-tabs>
    <v-avatar size="36px">
      <v-img
        alt="Avatar"
        src="https://avatars0.githubusercontent.com/u/9064066?v=4&s=460"
      ></v-img>
    </v-avatar>

    <v-btn icon="mdi-chevron-down" variant="text"></v-btn>
  </v-app-bar>
</template>

<script>
export default {};
</script>

<style></style>
