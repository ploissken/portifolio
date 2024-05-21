<template>
  <v-container class="fill-height">
    <v-row>
      <v-spacer />
      <v-col
        v-for="{ icon, href } in buttonsData"
        class="d-flex justify-center"
        :key="href"
      >
        <v-btn size="x-large" target="_blank" :icon="icon" :href="href" />
      </v-col>
      <v-spacer />
    </v-row>
  </v-container>
</template>

<script setup lang="ts">
const buttonsData = [
  { icon: "mdi-github", href: "https://github.com/ploissken?tab=repositories" },
  {
    icon: "mdi-stack-overflow",
    href: "https://stackoverflow.com/users/9866878/rodurico",
  },
  {
    icon: "mdi-linkedin",
    href: "https://www.linkedin.com/in/rodrigo-souza-97302724/",
  },
];
</script>
