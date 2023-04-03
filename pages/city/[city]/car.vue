
import Card from '~~/components/Car/card.vue';
<script setup>
import { useutilities } from '~~/pages/composables/useutilities';

const route = useRoute();
const{toTitleCase} = useutilities();
useHead({
    title: toTitleCase(route.params.city),
});

definePageMeta({
 layout : "custom",
});

</script>
<template>
    <div>
  <div class="mt-32 flex">
    <div class="shadow border w-64 mr-10 z-30 h-[190px]">
      <div class="p-5 flex justify-between relative cursor-pointer border-b">
        <h3>Location</h3>
        <h3 class="text-blue-400 capitalize">Toronto</h3>
     
      </div>

      <div class="p-5 flex justify-between relative cursor-pointer border-b">
        <h3>Make</h3>
        <h3 class="text-blue-400 capitalize">Toyota</h3>
      </div>

      <div class="p-5 flex justify-between relative cursor-pointer border-b">
        <h3>Price</h3>
        <h3 class="text-blue-400 capitalize"></h3>

    </div>

    </div>
    <NuxtPage />
</div>

</div>


</template>

