<template>
    <div class="min-h-screen py-6 flex flex-col text-gray-800 justify-center relative overflow-hidden sm:py-12">
        <div class="relative py-3 sm:max-w-xl mx-auto">
            <p class="text-2xl my-4">Login to your account</p>
            <div class=" p-3 rounded-md border border-gray-300">
                <form>
                    <div class="mb-4 text-gray-700">
                        <label class="block mb-1" for="username">Username</label>
                        <input class="w-full h-10 px-3 text-base border rounded-lg focus:outline-none focus:border-gray-700" type="text" id="username" />
                    </div>  
                    <div class="mb-4 text-gray-700">
                        <label class="block mb-1" for="passwordField">Password</label>
                        <input class="w-full h-10 px-3 text-base border border-red-700 rounded-lg focus:outline-none focus:border-gray-700" type="password" id="passwordField"/>
                        <span class="text-xs text-red-700">Your password is too short.</span>
                    </div>
                    <div class="mb-4">
                        <button class="block bg-green-600 rounded-md text-white p-2 w-full hover:shadow-md">Sign in</button>
                    </div>
                </form>
            </div>
        </div>
    </div>
</template>

<script lang="ts">

import { Component, Vue } from 'vue-property-decorator';

@Component
export default class Login extends Vue {}

</script>