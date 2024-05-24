<template>
  <div>
    {{ count }}
  </div>
</template>
<script setup>
import { useExampleStore } from "@/store/example";
import { storeToRefs } from "pinia";

const exampleStore = useExampleStore();
const { count } = storeToRefs(exampleStore);
</script>
