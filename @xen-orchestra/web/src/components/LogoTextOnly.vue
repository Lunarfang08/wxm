<template>
  <svg
    :class="{ short }"
    :viewBox="short ? '65 622 125 64' : '65 622 735 64'"
    class="logo-text-only"
    xmlns="http://www.w3.org/2000/svg"
  >
    <g>
      <!-- W -->
      <polygon points="120.48 684.92 106.08 684.92 92.38 664.14 80.22 684.92 66.35 684.92 82.14 659.25 103.51 659.25 120.48 684.92" />
      
      <!-- X -->
      <polygon points="119.54 624.06 104.07 649.22 82.04 649.22 65.41 624.06 79.81 624.06 93.51 644.84 105.66 624.06 119.54 624.06" />
      
      <!-- M -->
      <path d="M180 624.07v60.84h-12.15v-36l-10.92 22.5-10.92-22.5v36h-12.15v-60.84h14.47l8.6 17.3 8.6-17.3H180Z" />
    </g>
  </svg>
</template>

<script lang="ts" setup>
defineProps<{ short?: boolean }>()
</script>

<style lang="postcss" scoped>
.logo-text-only {
  fill: var(--color-neutral-txt-primary);
}

.short {
  .o {
    transform: translateX(-140px);
  }

  .long-only {
    display: none;
  }
}
</style>
