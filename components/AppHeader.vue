<template>
    <div class="shrink-0 flex w-full h-[61px] max-w-[1116px] justify-between items-center sm:items-end mx-auto py-1 mt-[8px]">
        <div class=" flex gap-3 items-end">
            <div class="border-b-4 border-primary sm:hover:bg-primary sm:hover:text-white sm:dark:hover:text-black">
                <NuxtLink to="/">
                    <p class="text-xl sm:text-2xl">Ahmad Aiman Alias</p>
                </NuxtLink>
            </div>
            <div class="hidden sm:block hover:bg-primary hover:text-white dark:hover:text-black">
                <NuxtLink>
                    <Icon name="radix-icons:github-logo" size="1.75em" />
                </NuxtLink>
            </div>
            <div class="hidden sm:block hover:bg-primary hover:text-white dark:hover:text-black">
                <NuxtLink>
                    <Icon name="radix-icons:linkedin-logo" size="1.75em" />
                </NuxtLink>
            </div>
        </div>
        <div class="hidden sm:flex text-lg gap-6 items-end">
            <p class="border-b-4 border-primary hover:bg-primary hover:text-white dark:hover:text-black">
                <NuxtLink to="/projects">
                    <span>/</span>projects
                </NuxtLink>
            </p>
            <p class="border-b-4 border-primary hover:bg-primary hover:text-white dark:hover:text-black" >
                <NuxtLink to="/blogs">
                    <span>/</span>blogs
                </NuxtLink>
            </p>
            <div>
                <ThemeToggle />
            </div>
        </div>
        <div class="sm:hidden">
            <MenuPopover />
        </div>
    </div>
</template>