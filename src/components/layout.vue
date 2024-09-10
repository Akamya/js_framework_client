<script setup>
import Nav from "./nav.vue";
import Footer from "./footer.vue";
</script>

<template>
  <div class="flex flex-col min-h-screen">
    <header>
      <Nav></Nav>
    </header>

    <main class="flex-grow py-5">
      <div class="container mx-auto">
        <slot name="title" />
        <slot name="content" />
        <slot></slot>
      </div>
    </main>

    <Footer></Footer>
  </div>
</template>
