<script setup lang="ts">
import {
  Popover,
  PopoverContent,
  PopoverTrigger,
} from '@/components/ui/popover'
import { Button } from '@/components/ui/button'

</script>

<template>
  <Popover>
    <PopoverTrigger as-child>
      <Button variant="ghost">
        <Icon name="tabler:menu-deep" size="2em" />
      </Button>
    </PopoverTrigger>
    <PopoverContent 
    align="end"
    class="w-60">
        <div class="text-lg gap-6 items-end mt-2">
            <h1 class="mb-4">
                <NuxtLink to="/projects" class="border-b-4 border-primary" >
                    <span>/</span>projects
                </NuxtLink>
            </h1>
            <h1 class="my-4 " >
                <NuxtLink to="/blogs" class="border-b-4 border-primary" >
                    <span>/</span>blogs
                </NuxtLink>
            </h1>
            <div class="mt-10 space-x-4">
                <NuxtLink>
                    <Icon name="radix-icons:github-logo" size="1.75em" />
                </NuxtLink>
                <NuxtLink>
                    <Icon name="radix-icons:linkedin-logo" size="1.75em" />
                </NuxtLink>
            </div>
            <div class="mt-4">
                <ThemeToggle />
            </div>
        </div>
    </PopoverContent>
  </Popover>
</template>