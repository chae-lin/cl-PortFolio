<script setup>
useHead({
  meta: [{ name: "viewport", content: "width=device-width, initial-scale=1" }],
  link: [{ rel: "icon", href: "/favicon.png" }],
  htmlAttrs: {
    lang: "en",
  },
});

const title = "Chaelin Kim | Frontend Developer";
const description =
  "사용자 경험을 중심으로 접근성과 성능을 고려한 UI를 구현하는 프론트엔드 개발자입니다. 섬세한 마크업과 안정적인 구조 설계를 지향합니다.";

useSeoMeta({
  title,
  description,
  ogTitle: title,
  ogDescription: description,
  ogImage: "https://ui.nuxt.com/assets/templates/nuxt/starter-light.png",
  twitterImage: "https://ui.nuxt.com/assets/templates/nuxt/starter-light.png",
  twitterCard: "summary_large_image",
});
</script>

<template>
  <div class="app">
    <LayoutHeader />
    <NuxtPage />
    <LayoutFooter />
  </div>
</template>

<style scoped>
.app {
  @apply flex flex-col min-h-[100vh] bg-[url(/images/intro/bg.jpeg)] bg-repeat;
}
main {
  @apply flex-1;
}
</style>
