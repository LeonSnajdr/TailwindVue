<template>
    <div class="w-full md:w-1/4 border rounded-lg shadow-sm m-4">
        <div class="p-4">
            <div class="flex flex-row justify-between mb-2">
                <h2 class="text-lg text-black font-bold">Projects</h2>
                <button class="px-4 py-1 bg-blue-100 hover:bg-blue-200 rounded-md text-blue-400 font-bold flex items-center">
                    <svg width="20" height="20" fill="currentColor" aria-hidden="true">
                        <path d="M10 5a1 1 0 0 1 1 1v3h3a1 1 0 1 1 0 2h-3v3a1 1 0 1 1-2 0v-3H6a1 1 0 1 1 0-2h3V6a1 1 0 0 1 1-1Z" />
                    </svg>
                    New
                </button>
            </div>
            <div class="relative mb-4">
                <svg width="20" height="20" fill="currentColor" class="absolute left-3 top-1/2 transform -translate-y-1/2 text-gray-400">
                    <path fill-rule="evenodd" clip-rule="evenodd" d="M8 4a4 4 0 100 8 4 4 0 000-8zM2 8a6 6 0 1110.89 3.476l4.817 4.817a1 1 0 01-1.414 1.414l-4.816-4.816A6 6 0 012 8z" />
                </svg>
                <input class="focus:border-light-blue-500 focus:ring-1 focus:ring-light-blue-500 focus:outline-none w-full text-sm text-black placeholder-gray-500 border border-gray-200 rounded-md py-2 pl-10" type="text" aria-label="Filter projects" placeholder="Filter projects" />
            </div>
        </div>
        <div class="grid grid-cols-2 gap-4 bg-gray-50 p-4">
            <ProjectItem title="Test" subTitle="Du kencht" />
            <ProjectItem title="Hallo" subTitle="Bomben ding" />
            <div class="group w-full border border-solid hover:border-dashed rounded-md p-4 border-gray-200 hover:border-blue-500 hover:bg-white flex flex-col items-center justify-center">
                <svg class="group-hover:text-blue-500 mb-1 text-gray-500" width="20" height="20" fill="currentColor" aria-hidden="true">
                    <path d="M10 5a1 1 0 0 1 1 1v3h3a1 1 0 1 1 0 2h-3v3a1 1 0 1 1-2 0v-3H6a1 1 0 1 1 0-2h3V6a1 1 0 0 1 1-1Z" />
                </svg>
                <p class="text-sm text-gray-500 group-hover:text-blue-500">Add a project</p>
            </div>
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