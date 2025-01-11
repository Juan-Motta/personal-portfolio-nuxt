<template>
  <button @click="toogleTheme" class="align-middle hover:bg-[var(--hover-nav)] rounded-full p-2">
    <span>
      <component
        :is="currentIcon"
        class="h-[40px] w-[40px] md:h-[28px] md:w-[28px]"
      />
    </span>
  </button>
</template>

<script setup>
import { defineAsyncComponent, computed} from 'vue'

const colorMode = useColorMode();

const IconsMoon = defineAsyncComponent(() => import('@/components/icons/moon.vue'))
const IconsSun = defineAsyncComponent(() => import('@/components/icons/sun.vue'))

const icons = {
  dark: IconsMoon,
  light: IconsSun,
}

function toogleTheme(event) {
  colorMode.value = colorMode.value === 'dark' ? 'light' : 'dark';
}

const currentIcon = computed(() => {
  return icons[colorMode.value];
});

</script>