<template>
    <div class="tw-w-[390px] tw-mx-auto tw-h-[100vh] tw-bg-white tw-px-4">
        <NuxtLink to="/"><p>back</p></NuxtLink>
        <h1 class="tw-pt-4 tw-text-[20px]">Вход</h1>
        <Inputform labelName="Электронная почта или телефон" placeholderName="taptym@gmail.com" idname="login" />
        <Inputform labelName="Пароль" placeholderName="••••••••••" idname="password" />
        <button class="tw-bg-[#E5E5EA] tw-rounded-[16px] tw-w-full tw-h-[48px] tw-mt-4 tw-text-white">Войти</button>
    </div>
</template>

<script setup>
definePageMeta({
    layout:'auth'
})
import Inputform from '~/components/auth/inputform.vue';


</script>
