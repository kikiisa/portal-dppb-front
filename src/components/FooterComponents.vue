<template>
  <footer
    class="footer footer-horizontal footer-center p-10 dark:bg-slate-900 bg-base-200 rounded-2xl m-3"
  >
    <aside>
      <div class="flex flex-wrap gap-2">
        <img width="50" src="../assets/logo-kemendukbangga.png" alt="logo-kemendukbangga">
        <img width="50" src="../assets/bglimboto.png" alt="logo-gorontalo">
      </div>
      <p class="font-bold dark:text-white">
        DPPKB KAB GORONTALO
        <br />
        
      </p>
      <p class="dark:text-white">Copyright © TIM IT DALDUK {{ new Date().getFullYear() }} - All right reserved</p>
    </aside>
    <nav>
      <div class="grid grid-flow-col gap-4">
      
        <a>
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="24"
        
            viewBox="0 0 24 24"
            class="fill-current dark:text-primary"
          >
            <path
              d="M19.615 3.184c-3.604-.246-11.631-.245-15.23 0-3.897.266-4.356 2.62-4.385 8.816.029 6.185.484 8.549 4.385 8.816 3.6.245 11.626.246 15.23 0 3.897-.266 4.356-2.62 4.385-8.816-.029-6.185-.484-8.549-4.385-8.816zm-10.615 12.816v-8l8 3.993-8 4.007z"
            ></path>
          </svg>
        </a>
        <a>
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="24"
            viewBox="0 0 24 24"
            class="fill-current dark:text-primary"
          >
            <path
              d="M9 8h-3v4h3v12h5v-12h3.642l.358-4h-4v-1.667c0-.955.192-1.333 1.115-1.333h2.885v-5h-3.808c-3.596 0-5.192 1.583-5.192 4.615v3.385z"
            ></path>
          </svg>
        </a>
      </div>
    </nav>
  </footer>
</template>
