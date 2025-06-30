<script setup>
import NavbarComponents from "./components/NavbarComponents.vue";
import HeroComponents from "./components/HeroComponents.vue";
import CardComponents from "./components/CardComponents.vue";
</script>

<template>
  <main class="lg:w-1/2 mx-auto">
    <NavbarComponents />
    <HeroComponents />
    <div class="text-center text-2xl font-bold dark:text-white">
      Menu <span class="text-primary">Utama</span>
    </div>
    <div class="grid lg:grid-cols-2 justify-center items-center gap-4 mt-4 p-3">
      <CardComponents
        link="https://drive.google.com/drive/folders/1uxJD4v8O6KmKT_iW3wMDqcWCvOt9L0nu"
        name="Materi "
        description="Slide Materi Workshop Peningkatan  kompetensi pengelola 
Kampung Keluarga Berkualitas  dan 
Rumah Data Kependudukan"
      />
      <CardComponents
        link="https://drive.google.com/drive/folders/1cXsz-Fk4sBdFbnmtoGW5nmojehbtoK20?usp=sharing"
        name="Sertifikat "
        description="Sertifikat Workshop Peningkatan  kompetensi pengelola 
Kampung Keluarga Berkualitas  dan 
Rumah Data Kependudukan"
      />
      <!-- <CardComponents name="Tugas"/> -->
    </div>
  </main>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
