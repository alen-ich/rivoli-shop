<template>
  <div class="relative flex flex-col items-center pt-[246px]">
    <img src="@/assets/logo-back.svg" class="absolute top-0 -right-[200px]" alt="" />
    <h4 class="text-[60px] uppercase font-semibold font-cormorant">{{ $t('home.gallery') }}</h4>
    <div class="grid grid-cols-5 items-center gap-8 px-16 mt-[120px]">
      <div class="flex flex-col items-center gap-6 col-span-2">
        <div class="flex flex-col gap-4">
          <img src="@/assets/pre-gallery-1.png" width="384" height="586" alt="" />
        </div>
        <div class="flex flex-col gap-4">
          <img src="@/assets/pre-gallery-2.png" width="384" height="586" alt="" />
        </div>
      </div>
      <div class="flex flex-col gap-4 col-span-3">
        <img src="@/assets/pre-gallery-3.png" width="716" height="716" alt="" />
      </div>
    </div>
    <PageLink :route="{ name: 'gallery' }" :text="$t('pageLink.gallery')" has-margin />
  </div>
</template>

<script setup lang="ts">
import { PageLink } from '@/shared'
</script>
