<template>
  <div class="tw-w-[390px] tw-mx-auto tw-bg-white tw-border-t-[1px] tw-flex tw-items-center tw-justify-between tw-p-3">
    <div class="tw-flex tw-flex-col tw-items-center tw-gap-1">
      <img class="tw-h-[22px] tw-w-[22px]" src="/home.png" alt="" />
      <span class="tw-text-[10px] tw-text-[#8E8E93]">Продаю</span>
    </div>
    <Nuxtlink to="/buy" class="tw-flex tw-flex-col tw-items-center tw-gap-1">
      <img class="tw-h-[22px] tw-w-[22px]" src="/buy.png" alt="" />
      <span class="tw-text-[10px] tw-text-[#8E8E93]">Куплю</span>
    </Nuxtlink>
    <div class="tw-flex tw-flex-col tw-items-center tw-gap-1">
      <img class="tw-h-[22px] tw-w-[22px]" src="/create.png" alt="" />
      <span class="tw-text-[10px] tw-text-[#8E8E93]">Создать</span>
    </div>
    <div class="tw-flex tw-flex-col tw-items-center tw-gap-1">
      <img class="tw-h-[22px] tw-w-[22px]" src="/message.png" alt="" />
      <span class="tw-text-[10px] tw-text-[#8E8E93]">Сообщения</span>
    </div>
    <NuxtLink to="/login" class="tw-flex tw-flex-col tw-items-center tw-gap-1">
      <img class="tw-h-[22px] tw-w-[22px]" src="/profile.png" alt="" />
      <span class="tw-text-[10px] tw-text-[#8E8E93]">Профиль</span>
    </NuxtLink>
  </div>
</template>

<script setup></script>
