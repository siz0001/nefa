<template>
  <div class="w-full lg:w-1/3 mt-6 lg:mt-0 overflow-hidden space-y-6 flex flex-col" v-bind="$attrs"  >
    <div class="w-full flex items-center justify-center" style="font-size:18px">
      {{ title }}
      <!-- <button
        href="#"
        class="px-3 py-1 text-sm font-medium text-blue-500 flex items-center space-x-1 rounded-md hover:bg-blue-50 transition duration-300"
      >
        <span>More</span>
        <ChevronRightIcon :size="16" />
      </button> -->
    </div>
    <div class="flex flex-col justify-center">
      <div class="-my-2 overflow-x-auto sm:-mx-6 lg:-mx-8" style="font-size:16px">
        <div class="px-2 sm:px-6 py-2 align-middle inline-block min-w-full overflow-hidden">
          <div v-for="data in datasets" :key="data.id" class="text-center">
            {{ data.text }}
          </div>
        </div>
        <div class="px-2 sm:px-6 py-2 align-middle inline-block min-w-full overflow-hidden">
          <div v-for="data in datasets" :key="data.id" class="text-center" style="font-weight:700">
            {{ data.detail }}
          </div>
        </div>
          <!-- <table class="min-w-full">
            <thead>
              <tr>
                <th class="text-left text-sm font-medium text-gray-500">Name</th>
                <th class="text-left text-sm font-medium text-gray-500">Price</th>
                <th class="hidden sm:block text-left text-sm font-medium text-gray-500">Chart</th>
              </tr>
            </thead>
            <tbody>
              <tr v-for="data in datasets" :key="data.id" class="border-b border-gray-200">
                <td class="py-4 whitespace-nowrap">
                  <div class="flex items-center space-x-2">
                    <img :src="require(`~/assets/img/crypto-icon/${data.logo}`)" alt="" />
                    <span>{{ data.name }}</span>
                  </div>
                </td>
                <td class="py-4 whitespace-nowrap">
                  <div class="flex items-center">
                    <PlusThickIcon v-if="data.increase" :size="14" class="text-emerald-500" />
                    <MinusThickIcon v-else :size="14" class="text-red-500" />
                    <span>${{ data.price }}</span>
                  </div>
                </td>
                <td class="hidden sm:block whitespace-nowrap">
                  <div>
                    <LineChart class="w-28 h-12 -mx-2" :datasets="data.data" :increase="data.increase" />
                  </div>
                </td>
              </tr>
            </tbody>
          </table> -->

      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'LandingCryptoStatistic',
  props: {
    title: {
      type: String,
      default: '',
    },
    datasets: {
      type: Array,
      default: () => [],
    },
  },
}
</script>
