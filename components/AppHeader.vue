<template>
    <div class="shrink-0 flex w-full h-[61px] max-w-[1116px] justify-between items-end mx-auto py-1 mt-[8px]">
        <div class="flex gap-3 items-end">
            <NuxtLink to="/">
                <h1 class="text-2xl">Ahmad Aiman Alias</h1>
            </NuxtLink>
            <div >
                <Icon name="radix-icons:github-logo" size="1.75em"/>
            </div>
            <div>
                <Icon name="radix-icons:linkedin-logo" size="1.75em"/>
            </div>
        </div>
        <div class="flex text-lg gap-6 items-end">
            <NuxtLink to="/projects">
                <h1><span>/</span>projects</h1>
            </NuxtLink>
            <NuxtLink to="/blogs">
                <h1><span>/</span>blogs</h1>
            </NuxtLink>
            <div>
                <ThemeToggle />
            </div>
        </div>
    </div>
</template>