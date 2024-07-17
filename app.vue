<template>
  <div>
    <NuxtLayout>
      <NuxtPage />
    </NuxtLayout>
  </div>
</template>

<script setup lang="ts">

useHead({
  title: 'Ahmad Aiman Alias | Aspiring Web Developer',

  meta: [
  { charset: 'utf-8' },
  { name: 'viewport', content: 'width=device-width, initial-scale=1' },
  { hid: 'description', name: 'description', content: 'Professional web developer specializing in responsive design and custom web applications' },
  { name: 'keywords', content: 'web developer, front-end developer, back-end developer, full-stack developer' },
],

  link: [
    { rel: 'apple-touch-icon', sizes: '180x180', href: 'apple-touch-icon.png' },
    { rel: 'icon', type: 'image/png', sizes: '32x32', href: 'favicon-32x32.png' },
    { rel: 'icon', type: 'image/png', sizes: '16x16', href: 'favicon-16x16.png' },
    { rel: 'manifest', href: 'site.webmanifest' },
    { rel: 'canonical', href: 'https://ahmdaimn.xyz' }
  ]

})

</script>