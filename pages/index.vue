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
  <section class="sm:mx-auto w-full max-w-[1116px] mt-12">
    <div class="sm:flex justify-between">
      <div class="flex-1 text-xl">
        <h2 class="text-4xl mb-5">Pleased to meet you<span class="text-7xl text-primary">.</span></h2>
        <VueTypedJs :strings=positions :typeSpeed="100" :backSpeed="100" :loop="true" class="sm:hidden">
          <p class="text-2xl ">I'm a
            <span class="typing text-primary"></span>
          </p>
        </VueTypedJs>
        <VueTypedJs :strings=positions :typeSpeed="100" :backSpeed="100" :loop="true" class="hidden sm:block ">
          <p class="hidden sm:block text-2xl">Aspired to be a
            <span class="typing text-primary"></span>
          </p>
        </VueTypedJs>

        <p class="mt-2 text-base text-slate-500">Passionate about programming and web applications from front to back.
          Whether it's developing smooth user interfaces or building robust server-side logic, I enjoy every step of the
          process. Currently, I'm honing my skills in javascript/typescript, php and c# ecosystem with deep interest in
          cloud and self hosted solutions.</p>
      </div>
      <div class="flex-1 m-2 p-2 flex justify-center items-center rounded-lg">
        <NuxtImg src="/self_picture.png" alt="Ahmad Aiman Alias" width="300" height="300" class="rounded-md"
          placeholder />
      </div>
    </div>

    <!-- section for project -->
    <div class="mt-10 mb-20">
      <h2 class="text-3xl">Recent Projects<span class="text-7xl text-primary">.</span></h2>
      <JobCards />
    </div>

    <div class="max-w-[1000px] mt-10 text-base">
      <h2 class="text-3xl">Skills<span class="text-6xl text-primary">.</span></h2>
      <div class="my-2">
        <p class="underline decoration-primary decoration-4">
          #Frontend
        </p>
        <div class="grid grid-cols-3 sm:grid-cols-6 mt-2">
          <li v-for="item in frontend" :key="item" class="flex flex-col m-2">
            <Icon :name="`tabler:brand-${item}`" size="3rem" />
            <p class="text-wrap text-slate-500">
              {{ item }}
            </p>
          </li>
        </div>
      </div>
      <div class="my-3">
        <p class="underline decoration-primary decoration-4">
          #Backend
        </p>
        <div class="grid grid-cols-3 sm:grid-cols-6 mt-2">
          <li v-for="item in backend" :key="item" class="flex flex-col m-2">
            <Icon :name="`simple-icons:${item}`" size="3rem" />
            <p class="break-words text-slate-500">
              {{ item }}
            </p>
          </li>
        </div>
      </div>
      <div class="my-3">
        <p class="underline decoration-primary decoration-4">
          #Styling
        </p>
        <div class="grid grid-cols-3 sm:grid-cols-6 mt-2">
          <li v-for="item in styling" :key="item" class="flex flex-col m-2">
            <Icon :name="`simple-icons:${item}`" size="3rem" />
            <p class="text-wrap text-slate-500">
              {{ item }}
            </p>
          </li>
        </div>
      </div>
      <div class="my-3">
        <p class="underline decoration-primary decoration-4">
          #Others
        </p>
        <div class="grid grid-cols-3 sm:grid-cols-6 mt-2">
          <li v-for="item in others" :key="item" class="flex flex-col m-2">
            <Icon :name="`simple-icons:${item}`" size="3rem" />
            <p class="text-wrap text-slate-500">
              {{ item }}
            </p>
          </li>
          <li class="flex flex-col m-2">
            <Icon name="tabler:brand-azure" size="3rem" />
            <p class="text-wrap text-slate-500">
              azure
            </p>
          </li>
        </div>

      </div>
    </div>
    <div class="mt-10 mb-20">
      <h2 class="text-3xl">Contacts<span class="text-7xl text-primary">.</span></h2>
      <div class="sm:flex justify-between">
        <p class="max-w-[500px] my-2 text-slate-500">
          Currently looking for fulltime/freelance. However, if you have other request or question, don’t hesitate to
          contact me</p>
        <div>
          <p class="mt-10 sm:mt-0 text-primary">Message me here</p>
          <div class="flex items-center space-x-2">
            <Icon name="radix-icons:envelope-closed" size="1rem" />
            <NuxtLink to="mailto:ahmadaimanalias.gmail">
              <p>ahmadaimanalias.gmail</p>
            </NuxtLink>
          </div>
          <div class="flex items-center space-x-2">
            <Icon name="radix-icons:linkedin-logo" size="1rem" />
            <NuxtLink to="https://www.linkedin.com/in/ahmdaimnalias/" target="_blank">
              <p>ahmadaimnalias</p>
            </NuxtLink>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>