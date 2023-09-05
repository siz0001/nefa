<template>
  <div class="relative max-w-screen-xl mx-auto grid grid-cols-12 gap-x-6 overflow-hidden" v-bind="$attrs"><!-- px-4 sm:px-8 -->
    <slot></slot>
  </div>
</template>
<script>
export default {
  name: 'BaseSection',
}
</script>
