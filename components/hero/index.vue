<template>
  <section
    class="flex flex-col justify-center items-center md:gap-20 gap-10"
    :style="{ height: 'calc(100vh - 80px)' }"
  >
    <span class="text-xl md:text-3xl select-none font-bold">
      Hola, 👋🏻 soy
    </span>
    <h1
      class="backgroud-text text-7xl md:text-9xl break-words font-bold animate-gradient select-none text-center"
    >
      Juan Motta
    </h1>
    <span class="text-xl md:text-3xl select-none font-bold text-center">
      Desarrollador web full stack.
    </span>
    <div class="flex gap-8 md:flex-row flex-col">
      <ButtonHero>
        <span class="flex items-center h-full">
          <IconsSend
            class="h-[26px] w-[26px] stroke-black dark:stroke-white stroke-[2.5] fill-none"
          />
        </span>
        Contactame
      </ButtonHero>
      <ButtonHero>
        <span class="flex items-center h-full">
          <IconsDownload
            class="h-[28px] w-[28px] stroke-black dark:stroke-white stroke-[2.5]"
          />
        </span>
        Descargar CV
      </ButtonHero>
    </div>
    <div class="flex gap-5">
      <NuxtLink
        to="https://github.com/Juan-Motta"
        rel="noopener noreferrer"
        target="_blank"
      >
        <IconsGithub
          class="stroke-black dark:stroke-white fill-none stroke-2 w-[48px] h-[48px] hover:scale-125 transition-transform hover:stroke-[#e73c7e] dark:hover:stroke-[#e73c7e]"
        />
      </NuxtLink>
      <NuxtLink
        to="https://www.linkedin.com/in/jualopezmo/"
        rel="noopener noreferrer"
        target="_blank"
      >
        <IconsLinkedin
          class="stroke-black dark:stroke-white fill-none stroke-2 w-[48px] h-[48px] hover:scale-125 transition-transform hover:stroke-[#e73c7e] dark:hover:stroke-[#e73c7e]"
        />
      </NuxtLink>
      <ButtonSocial>
        <IconsMail
          class="stroke-black dark:stroke-white fill-none stroke-2 w-[48px] h-[48px] hover:scale-125 transition-transform hover:stroke-[#e73c7e] dark:hover:stroke-[#e73c7e]"
        />
      </ButtonSocial>
    </div>
  </section>
</template>

<style scoped>
.animate-gradient {
  animation: animatedgradient 6s ease infinite alternate;
}

.backgroud-text {
  background: -webkit-linear-gradient(
    -45deg,
    #ee7752,
    #e73c7e,
    #23a6d5,
    #23d5ab
  );
  background-size: 250%;
  -webkit-background-clip: text;
  background-clip: text;
  -webkit-text-fill-color: transparent;
}

@keyframes animatedgradient {
  0% {
    background-position: 0% 50%;
  }
  50% {
    background-position: 100% 50%;
  }
  100% {
    background-position: 0% 50%;
  }
}
</style>
