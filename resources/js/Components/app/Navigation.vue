<script setup>
import ApplicationLogo from '../ApplicationLogo.vue';
import CreateNewDropDown from '@/Components/app/CreateNewDropDown.vue'
import { Link } from '@inertiajs/vue3';
import NavLink from '../NavLink.vue';
</script>

<template>
    <nav class="min-w-[200px]">
        <div class="h-[80px] px-3 flex items-center gap-3">
            <Link href="/">
                <ApplicationLogo
                    class="block h-9 w-auto fill-current text-gray-800"
                  />
            </Link>
            LaraStorage
        </div>
        <div class="px-3">
            <CreateNewDropDown/>
            
            <div class="py-3">
                <NavLink href="/">My Files</NavLink>
                <NavLink href="/" :active="true">Shared with me</NavLink>
                <NavLink href="/">Shared by me</NavLink>
                <NavLink href="/">Trash</NavLink>
            </div>
        </div>
    </nav>
</template>
