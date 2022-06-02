<template>
  <div class="bg-white shadow">
    <div class="px-4 sm:px-6 lg:mx-auto lg:px-8">
      <div class="py-6 md:flex md:items-center md:justify-between lg:border-t lg:border-gray-200">
        <div class="flex-1 min-w-0">
          <slot />
        </div>

        <div class="mt-6 flex space-x-3 md:mt-0 md:ml-4">
          <slot name="buttons">
          <button type="button"
                  class="inline-flex items-center px-4 py-2 border border-gray-300 shadow-sm text-sm font-medium rounded-md text-gray-700 bg-white hover:bg-gray-50 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-cyan-500">
            Add money
          </button>
          <button type="button"
                  class="inline-flex items-center px-4 py-2 border border-transparent shadow-sm text-sm font-medium rounded-md text-white bg-cyan-600 hover:bg-cyan-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-cyan-500">
            Send money
          </button>
          </slot>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import {CheckCircleIcon, OfficeBuildingIcon} from "@heroicons/vue/solid";

export default {
  components:{
    OfficeBuildingIcon,
    CheckCircleIcon,
  }

}
</script>
