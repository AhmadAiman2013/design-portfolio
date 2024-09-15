<script lang="ts" setup>
import {
  Card,
  CardContent,
  CardDescription,
  CardHeader,
  CardTitle,
} from '@/components/ui/card'
</script>

<template>
    <NuxtLink to="https://coret.ahmdaimn.xyz/" target="_blank">
        <Card class="w-[250px] my-2 sm:w-[350px]">
          <div>
            <NuxtImg src="/coret_screenshot.png" alt="Coret"  class="rounded-md" placeholder />
          </div>
          <CardHeader>
            <CardTitle>Coret</CardTitle>
            <CardDescription>Simple, lean and all-around task manager</CardDescription>
          </CardHeader>
          <CardContent>
            <p>Experience absolute fast and well-crafted note taking application. Powered by Nextjs, Laravel and AWS.</p>
          </CardContent>
        </Card>
      </NuxtLink>
</template>
