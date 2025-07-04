<script setup>
import { onMounted, ref } from 'vue';
const isDark = ref(false);
const toggleDarkMode = () => {
    console.log(isDark.value);
  if (document.documentElement.classList.contains("dark")) {
    document.documentElement.classList.remove("dark");
    localStorage.setItem("theme", "light");
    isDark.value = false;
  } else {
    document.documentElement.classList.add("dark");
    localStorage.setItem("theme", "dark");
    isDark.value = true;
  }
};
onMounted(() => {
  const theme = localStorage.getItem("theme");
  if (theme === "dark") {
    document.documentElement.classList.add("dark");
    isDark.value = true;
  } else {
    document.documentElement.classList.remove("dark");
    isDark.value = false;
  }
});
</script>
<template>
  <div class="mt-4 rounded-2xl p-3">
    <div class="flex justify-between items-center dark:bg-slate-800 bg-base-200 p-3 rounded-2xl shadow-xl">
      <a class="btn btn-ghost normal-case text-xl text-center dark:text-white" href="/">
         <img width="40" src="../assets/logo-kemendukbangga.png" alt="logo-kemendukbangga">
         <img width="40" src="../assets/bglimboto.png" alt="logo-gorontalo">
      </a>
      <div class="theme-control">
        <label class="flex cursor-pointer gap-2">
          <svg
        
            xmlns="http://www.w3.org/2000/svg"
            width="20"
            height="20"
            viewBox="0 0 24 24"
            class="dark:text-white"
            fill="none"
            stroke="currentColor"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round"
          >
            <circle cx="12" cy="12" r="5" />
            <path
              d="M12 1v2M12 21v2M4.2 4.2l1.4 1.4M18.4 18.4l1.4 1.4M1 12h2M21 12h2M4.2 19.8l1.4-1.4M18.4 5.6l1.4-1.4"
            />
          </svg>
          <input
           @change="toggleDarkMode"
            
           :checked="isDark"
            type="checkbox"
            value="synthwave"
            class="toggle theme-controller"
          />
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="20"
            height="20"
            viewBox="0 0 24 24"
            fill="none"
            class="dark:text-white"
            stroke="currentColor"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round"
          >
            <path d="M21 12.79A9 9 0 1 1 11.21 3 7 7 0 0 0 21 12.79z"></path>
          </svg>
        </label>
      </div>
    </div>
  </div>
</template>
