<template>
  <div class="mb-6">
    <h2
      class="mt-6 text-4xl text-gray-700 font-bold capitalize dark:text-blue-200"
    >
      {{ authorIntro.headline }}
    </h2>
    <p class="mt-8 mb-4 dark:bg-gray-800 dark:text-blue-200 text-justify" v-for="(line, index) in authorIntro.introduction" :key="index">
      {{line}}
    </p>
  </div>
</template>
<script>
import authourIntro from "@/data/authorIntro"

export default {
  data: () => {
    return {
      authorIntro:authourIntro 
    }
  }
}
</script>