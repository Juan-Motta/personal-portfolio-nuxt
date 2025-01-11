<template>
  <nav class="mt-5 flex justify-between items-center md:flex-row flex-col">
    <div class="flex w-full justify-between md:w-auto z-20">
      <NuxtLink
        to="/"
        class="text-4xl font-extrabold text hover:scale-110 transition-scale duration-100 cursor-pointer whitespace-pre-wrap select-none"
        >{ juan }</NuxtLink
      >
    </div>
    <ClientOnly>
      <ul
        class="pt-12 text-3xl md:text-lg md:flex-row flex-col items-center gap-5 md:static absolute justify-evenly md:py-0 -top-[60rem] transition-all duration-300 md:transition-none md:duration-0 opacity-0 md:opacity-100 h-full w-full md:h-auto md:w-auto flex z-10 backdrop-blur-xl md:backdrop-blur-0"
      >
        <li
          class="hover:font-extrabold transition-scale duration-100 cursor-pointer select-none"
        >
          <NuxtLink to="/">Acerca de mí</NuxtLink>
        </li>
        <li
          class="hover:font-extrabold transition-scale duration-100 cursor-pointer select-none"
        >
          <NuxtLink to="/">Proyectos</NuxtLink>
        </li>
        <li
          class="hover:font-extrabold transition-scale duration-100 cursor-pointer select-none"
        >
          <NuxtLink to="/">Contácto</NuxtLink>
        </li>
        <li
          class="hover:font-extrabold transition-scale duration-100 cursor-pointer select-none"
        >
          <NuxtLink to="/">Blog</NuxtLink>
        </li>
        <li>
          <NavbarThemeToggler />
        </li>
      </ul>
    </ClientOnly>
  </nav>
</template>