<template>
    <div class="group w-full border rounded-md p-4 border-gray-200 bg-white hover:bg-blue-500 hover:text-white">
        <h2 class="text-lg">{{ title }}</h2>
        <p class="text-sm text-gray-500 group-hover:text-gray-200">{{ subTitle }}</p>
    </div>
</template>

<script lang="ts">

import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class ProjectItem extends Vue {

    @Prop(String) title!: string;
    @Prop(String) subTitle!: string;

}

</script>