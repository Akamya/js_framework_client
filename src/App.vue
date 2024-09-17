<script setup>
import Layout from "./Layout/layout.vue";
import PButton from "./components/primaryButton.vue";
import { RouterView } from "vue-router";
</script>

<template>
  <Layout>
    <template v-slot:title>
      <h1 class="mt-5 text-3xl font-bold">
        Pied de page fixe avec barre de navigation
      </h1>
    </template>

    <template v-slot:content>
      <p class="text-lg">
        Utilisez Tailwind pour fixer un pied de page au bas de la fenêtre avec
        des classes utilitaires comme
        <code class="bg-gray-200 text-sm p-1 rounded">min-h-screen</code> et
        <code class="bg-gray-200 text-sm p-1 rounded">flex flex-col</code>.
      </p>
      <p>
        Découvrez plus d'exemples en visitant
        <RouterView
          href="https://tailwindcss.com/docs"
          class="text-blue-500 hover:underline"
          >la documentation officielle de Tailwind CSS</RouterView
        >.
      </p>
    </template>
    <PButton>Cliquez ici</PButton>
    <RouterView></RouterView>
  </Layout>
</template>
