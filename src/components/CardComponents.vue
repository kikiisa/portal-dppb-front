<script setup>
    const props = defineProps({
        name: String,
        description: String,
        link:String
    });
</script>
<template>
  <div class="card card-border border-slate-300 hover: dark:border-slate-900 dark:bg-slate-900 lg:w-2/2 dark:hover:bg-slate-600 hover:bg-base-200">
    <div class="card-body">
      <h2 class="card-title">
        <svg
          class="w-6 h-6 dark:text-white"
          aria-hidden="true"
          xmlns="http://www.w3.org/2000/svg"
          width="24"
          height="24"
          fill="none"
          viewBox="0 0 24 24"
        >
          <path
            stroke="currentColor"
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M12 6.03v13m0-13c-2.819-.831-4.715-1.076-8.029-1.023A.99.99 0 0 0 3 6v11c0 .563.466 1.014 1.03 1.007 3.122-.043 5.018.212 7.97 1.023m0-13c2.819-.831 4.715-1.076 8.029-1.023A.99.99 0 0 1 21 6v11c0 .563-.466 1.014-1.03 1.007-3.122-.043-5.018.212-7.97 1.023"
          />
        </svg>
        <span class="dark:text-white">
            {{ props.name }}
        </span>
      </h2>
      <p class="dark:text-white">{{ props.description }}</p>
      <div class="card-actions justify-end">
        <a :href="props.link" class="btn btn-primary">Detail</a>
      </div>
    </div>
  </div>
</template>
