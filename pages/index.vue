<script setup lang="ts">
import { VueTypedJs } from 'vue3-typed-ts';

const positions = ['Frontend?', 'Backend?', 'Fullstack?', 'DevOps?'];
</script>

<template>
  <section class="w-full max-w-[1116px] mx-auto mt-12">
    <div class="flex justify-between">
      <div class="flex-1 text-xl">
        <h1 class="text-4xl mb-5">Pleased to meet you.</h1>
        <h2>Code. Create. and Code again.</h2>
        <VueTypedJs :strings=positions :typeSpeed="100" :backSpeed="100" :loop="true">
          <h2>Looking for
            <span class="typing"></span>
          </h2>
        </VueTypedJs>
        <p class="mt-5 text-base">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Itaque eius laboriosam
          deleniti sed, at in modi atque
          magnam laborum error. Eveniet qui sapiente harum voluptate voluptas in deserunt tenetur eius.</p>
      </div>
      <div class="flex-1 m-2 p-2 flex justify-center items-center rounded-lg">
        <NuxtImg src="/self_picture.png" alt="Ahmad Aiman Alias" width="300" height="300" class="rounded-md" />
      </div>
    </div>
    <div class="mt-10 text-base">
      <h1 class="text-3xl">Skills.</h1>
      <div class="my-2">
        <h1>
          #Frontend
        </h1>
        
      </div>
      <div class="my-2">
        <h1>
          #Backend
        </h1>
      </div>
      <div class="my-2">
        <h1>
          #Styling
        </h1>
      </div>
      <div class="my-2">
        <h1>
          #Others
        </h1>
      </div>
    </div>
    <div class="mt-10 mb-20">
      <h1 class="text-3xl">Contacts.</h1>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempora nisi nesciunt quibusdam totam suscipit ducimus
        possimus deserunt eius unde voluptatem temporibus similique odio, laboriosam, natus, voluptatum perferendis
        repellat consequatur omnis?</p>
    </div>
  </section>
</template>