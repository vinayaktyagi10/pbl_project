<script setup lang="ts">
import { ref, computed } from 'vue'

const days = ref(30)
const totalSize = computed(() => days.value * 50) // 50GB per day legacy
const savedSize = computed(() => (50 + (days.value - 1) * 0.2).toFixed(1)) // 50GB first day, 200MB after
const savings = computed(() => (totalSize.value - Number(savedSize.value)).toFixed(0))
</script>

<template>
  <div class="p-6 bg-gray-800/50 rounded-xl border border-white/10 shadow-xl">
    <div class="mb-4">
      <label class="block text-sm font-bold mb-2 text-blue-400">Projection Period: {{ days }} Days</label>
      <input type="range" v-model="days" min="1" max="365" class="w-full h-2 bg-gray-700 rounded-lg appearance-none cursor-pointer accent-pink-500">
    </div>

    <div class="grid grid-cols-2 gap-4 text-center">
      <div class="p-4 bg-red-900/20 rounded border border-red-500/30">
        <span class="block text-xs uppercase opacity-60">Legacy Storage</span>
        <span class="text-2xl font-bold">{{ totalSize }} GB</span>
      </div>
      <div class="p-4 bg-green-900/20 rounded border border-green-500/30">
        <span class="block text-xs uppercase opacity-60">Our Optimized System</span>
        <span class="text-2xl font-bold">{{ savedSize }} GB</span>
      </div>
    </div>

    <div class="mt-4 p-3 bg-[#50fa7b] rounded text-center font-bold text-[#282a36] shadow-lg">
      Total Savings: {{ savings }} GB
    </div>
  </div>
</template>
