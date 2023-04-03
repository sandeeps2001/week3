<script setup>
import { use } from 'h3';
const route = useRoute();
definePageMeta({
 layout : "custom",
});
const{toTitleCase} = useutilities();
useHead({
  title: toTitleCase(route.params.name),
});
</script>
<template>
   <div>
    <CardetailsHero />
  <div class="mr-10 mt-5 border-b pb-5">
    <div class="flex text-lg mt-2">
      <p class="rounded text-lime-800 mr-3">✔</p>
      <p>Leather Interior</p>
    </div>
  </div>
  <CardetailsDesc />
</div>
</template>