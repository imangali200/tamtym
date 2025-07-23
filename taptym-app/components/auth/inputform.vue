<template>
  <div class="tw-flex tw-flex-col tw-gap-2 tw-mt-3">
    <label :for="idname">{{props.labelName}}</label>
    <input
      class="tw-border-[1px] tw-h-[48px] tw-rounded-[16px] tw-px-3"
      :placeholder="props.placeholderName"
      type="text"
      :id="idname"
    />
  </div>
</template>

<script setup>
const props = defineProps({
  labelName: String,
  placeholderName: String,
  idname:String
});
console.log(props);
</script>

<style lang="scss" scoped></style>
