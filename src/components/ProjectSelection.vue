<template>
    <div class="w-full md:w-5/12 border p-4">
        <div class="flex flex-row justify-between mb-2">
            <h2 class="text-lg text-black font-bold">Projects</h2>
            <button class="px-4 py-1 bg-blue-100 hover:bg-blue-200 rounded-md text-blue-400 font-bold">+ New</button>
        </div>
        <div class="relative mb-4">
            <svg width="20" height="20" fill="currentColor" class="absolute left-3 top-1/2 transform -translate-y-1/2 text-gray-400">
                <path fill-rule="evenodd" clip-rule="evenodd" d="M8 4a4 4 0 100 8 4 4 0 000-8zM2 8a6 6 0 1110.89 3.476l4.817 4.817a1 1 0 01-1.414 1.414l-4.816-4.816A6 6 0 012 8z" />
            </svg>
            <input class="focus:border-light-blue-500 focus:ring-1 focus:ring-light-blue-500 focus:outline-none w-full text-sm text-black placeholder-gray-500 border border-gray-200 rounded-md py-2 pl-10" type="text" aria-label="Filter projects" placeholder="Filter projects" />
        </div>
        <div class="grid grid-cols-2 gap-4">
            <ProjectItem />
            <ProjectItem />
            <ProjectItem />
            <ProjectItem />
            <ProjectItem />
        </div>
    </div>
</template>

<script lang="ts">

import { Component, Vue } from 'vue-property-decorator';
import ProjectItem from "@/components/Projecttem.vue"

@Component({
    components: { ProjectItem  }
})
export default class ProjectSelection extends Vue {}

</script>