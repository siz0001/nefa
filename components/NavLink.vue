<template>
  <li class="w-full">
    [{{ name }}]<br>
    <a
      class="py-2 text-sm bg-transparent rounded-lg text-[#666666] hover:text-gray-900 focus:outline-none focus:shadow-outline"
      :href="url"
    >

      {{ detail }}
    </a>
  </li>
</template>
<script>
export default {
  props: {
    name: {
      type: String,
      required: true,
    },
    detail: {
      type: String,
      required: true,
    },
    url: {
      type: String,
      required: true,
    },
  },
}
</script>
