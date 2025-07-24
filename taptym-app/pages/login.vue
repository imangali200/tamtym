<template>
  <div class="tw-w-[390px] tw-mx-auto tw-h-[100vh] tw-bg-white tw-px-4">
    <NuxtLink to="/"><p>back</p></NuxtLink>
    <h1 class="tw-pt-4 tw-text-[20px]">Вход</h1>
    <Inputform
      labelName="Электронная почта или телефон"
      placeholderName="taptym@gmail.com"
      idname="login"
    />
    <Inputform
      labelName="Пароль"
      placeholderName="••••••••••"
      idname="password"
    />
    <button
      class="tw-bg-[#E5E5EA] tw-rounded-[16px] tw-w-full tw-h-[48px] tw-mt-4 tw-text-white"
    >
      Войти
    </button>
    <p>{{ pending }}</p>
    <p>{{ error }}</p>
    <p>{{ user }}</p>
    <button @click="goBuy">go to second page</button>
    <button @click="goMain">leave to the main page</button>
  </div>
</template>

<script setup>
definePageMeta({
  layout: "auth",
});
const { data, pending, error } = await useAsyncData("user", () => {
  return $fetch(
    "https://pk-api.adata.kz/api/v1/data/search?most_viewed_companies=0&keyword=030121500948"
  );
});
console.log(data, pending, error);
import Inputform from "~/components/auth/inputform.vue";

const user = useCookie("nameUser");

if (!user.value) {
  user.value = "Imangali";
}
const goBuy = async () => {
  await navigateTo("/buy");
};
onBeforeRouteLeave((to, from, next) => {
  const answer = window.confirm("Are you sure you want to leave?");
  if (answer) {
    next(); // allow
  } else {
    next(false); // cancel
  }
});
onNuxtReady(() => {
  console.log('Welcome Imangali! Your app is ready.')
    alert('already site was ready')
})
</script>
