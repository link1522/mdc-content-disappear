<script setup>
const flag = ref(false);
const md = computed(() => (flag.value ? "# flag is true" : "# flag is false"));
</script>

<template>
  <div>
    <button @click="flag = !flag">toggle</button>
    <MDC :value="md" />
  </div>
</template>
