<template>
  <div class="flex items-center gap-3">
    <div class="flex items-center justify-center border rounded-lg p-1.5">
      <UIcon :name="icon" />
    </div>
    <div class="flex flex-col">
      <h3 class="font-semibold">
        <ContentSlot name="title" />
      </h3>
      <span>
        <ContentSlot name="description" />
      </span>
    </div>
  </div>
</template>

<script lang="ts">
export default {
  name: 'HomeFeatureComponent',
  props: {
    icon: {
      type: String,
      default: 'i-ph-cursor-click',
    },
  },
}
</script>