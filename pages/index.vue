<script setup lang="ts">
import { VueTypedJs } from 'vue3-typed-ts';

const positions = ['Frontend', 'Backend', 'Fullstack', 'DevOps'];

// frontend
const frontend = ['javascript', 'typescript', 'php', 'c-sharp', 'python', 'react', 'nextjs', 'vue', 'nuxt'];

//backend
const backend = [
  'nodedotjs',
  'express',
  'nestjs',
  'laravel',
  'dotnet',
  'fastapi',
  'mongodb',
  'postgresql',
  'mysql',
  'sqlite',
  'amazondynamodb',
  'microsoftsqlserver',
];

//styling
const styling = ['tailwindcss', 'postcss', 'bootstrap', 'daisyui', 'shadcnui'];

//others
// cloudflare,prisma,drizzle,git,figma,docker,terraform,aws,gcp,azure,langchain,pytorch
const others = ['cloudflare', 'prisma', 'drizzle', 'git', 'figma', 'langchain', 'pytorch', 'docker', 'terraform', 'amazonaws', 'googlecloud',];
</script>

<template>
  <section class="w-full max-w-[1116px] mx-auto mt-12">
    <div class="flex justify-between">
      <div class="flex-1 text-xl">
        <h1 class="text-4xl mb-5">Pleased to meet you<span class="text-7xl text-primary">.</span></h1>
        <VueTypedJs :strings=positions :typeSpeed="100" :backSpeed="100" :loop="true">
          <h1 class="text-2xl" >Aspired to be a
            <span class="typing text-primary"></span>
          </h1>
        </VueTypedJs>
        <p class="mt-2 text-base">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Itaque eius laboriosam
          deleniti sed, at in modi atque
          magnam laborum error. Eveniet qui sapiente harum voluptate voluptas in deserunt tenetur eius.</p>
      </div>
      <div class="flex-1 m-2 p-2 flex justify-center items-center rounded-lg">
        <NuxtImg src="/self_picture.png" alt="Ahmad Aiman Alias" width="300" height="300" class="rounded-md" />
      </div>
    </div>
    <div class="max-w-[1000px] mt-10 text-base">
      <h1 class="text-3xl">Skills<span class="text-6xl text-primary">.</span></h1>
      <div class="my-2">
        <h1 class="underline decoration-primary decoration-4" >
          #Frontend
        </h1>
        <div class="grid grid-cols-6 mt-2">
          <li v-for="item in frontend" :key="item" class="flex flex-col m-2">
            <Icon :name="`tabler:brand-${item}`" size="3rem" />
            {{ item }}
          </li>
        </div>
      </div>
      <div class="my-3">
        <h1 class="underline decoration-primary decoration-4" >
          #Backend
        </h1>
        <div class="grid grid-cols-6 mt-2">
          <li v-for="item in backend" :key="item" class="flex flex-col m-2">
            <Icon :name="`simple-icons:${item}`" size="3rem" />
            {{ item }}
          </li>
        </div>
      </div>
      <div class="my-3">
        <h1 class="underline decoration-primary decoration-4" >
          #Styling
        </h1>
        <div class="grid grid-cols-6 mt-2">
          <li v-for="item in styling" :key="item" class="flex flex-col m-2">
            <Icon :name="`simple-icons:${item}`" size="3rem" />
            {{ item }}
          </li>
        </div>
      </div>
      <div class="my-3">
        <h1 class="underline decoration-primary decoration-4" >
          #Others
        </h1>
        <div class="grid grid-cols-6 mt-2">
          <li v-for="item in others" :key="item" class="flex flex-col m-2">
            <Icon :name="`simple-icons:${item}`" size="3rem" />
            {{ item }}
          </li>
          <li class="flex flex-col m-2">
            <Icon name="tabler:brand-azure" size="3rem" />
            azure
          </li>
        </div>

      </div>
    </div>
    <div class="mt-10 mb-20">
      <h1 class="text-3xl">Contacts<span class="text-7xl text-primary">.</span></h1>
      <div class="flex justify-between" >
        <p class="max-w-[500px] my-2">
          Currently looking for fulltime/freelance. However, if you have other request or question, don’t hesitate to
          contact me</p>
        <div>
          <p class="text-primary" >Message me here</p>
          <div class="flex items-center space-x-2" >
            <Icon name="radix-icons:envelope-closed" size="1rem"/>
            <p>ahmadaimanalias.gmail</p>  
          </div>
          <div class="flex items-center space-x-2" >
            <Icon name="radix-icons:linkedin-logo" size="1rem"/>
            <p>ahmadaiman</p>  
          </div>
        </div>
      </div>
    </div>
  </section>
</template>