<template>
  <div class="flex items-center justify-between">
    <div class="flex-1 space-y-1.5">
      <h1 class="text-2xl font-bold">Alfredo Martínez</h1>
      <p
        class="max-w-md font-mono text-sm text-gray-500 text-pretty dark:text-gray-400"
      >
        {{ $t('intro.summary') }}
      </p>
      <p
        class="max-w-md items-center font-mono text-xs text-gray-500 text-pretty dark:text-gray-400"
      >
        <ULink
          class="inline-flex items-center leading-none gap-x-1.5 hover:underline"
          to="https://maps.app.goo.gl/N4AC13tG2Z6KThFN7"
          target="_blank"
        >
          <UIcon class="h-4 w-4" name="i-heroicons-globe-americas" dynamic />
          León, Gto. México, UTC-6
        </ULink>
      </p>
      <div
        class="flex print:hidden gap-x-1 pt-1 font-mono text-sm text-gray-500 dark:text-gray-400"
      >
        <UButton
          to="mailto:ialfredo.mtz.rmz@gmail.com"
          color="white"
          variant="solid"
        >
          <template #leading>
            <UIcon
              class="h-5 w-5 text-gray-500 dark:text-gray-400"
              name="i-ph-envelope-simple-duotone"
            />
          </template>
        </UButton>
        <UButton to="tel:+524776462056" color="white" variant="solid">
          <template #leading>
            <UIcon
              class="h-5 w-5 text-gray-500 dark:text-gray-400"
              name="i-ph-phone-duotone"
            />
          </template>
        </UButton>
        <UButton
          to="https://github.com/alfredomtzrmz"
          target="_blank"
          color="white"
          variant="solid"
        >
          <template #leading>
            <UIcon
              class="h-5 w-5 text-gray-500 dark:text-gray-400"
              name="i-ph-github-logo-duotone"
            />
          </template>
        </UButton>
        <UButton
          to="https://www.linkedin.com/in/alfredomtzrmz/"
          target="_blank"
          color="white"
          variant="solid"
        >
          <template #leading>
            <UIcon
              class="h-5 w-5 text-gray-500 dark:text-gray-400"
              name="i-ph-linkedin-logo-duotone"
            />
          </template>
        </UButton>
        <UButton
          to="https://twitter.com/alfredo_mtzrmz"
          target="_blank"
          color="white"
          variant="solid"
        >
          <template #leading>
            <UIcon
              class="h-5 w-5 text-gray-500 dark:text-gray-400"
              name="i-fa6-brands-x-twitter"
            />
          </template>
        </UButton>
      </div>
      <div
        class="print:flex hidden flex-col gap-x-1 font-mono text-sm text-gray-500 dark:text-gray-400"
      >
        <a href="mailto:ialfredo.mtz.rmz@gmail.com">
          <span class="underline">ialfredo.mtz.rmz@gmail.com</span> </a
        ><a href="tel:+524776462056"
          ><span class="underline">+524776462056</span></a
        >
      </div>
    </div>
    <span class="relative flex shrink-0 overflow-hidden rounded-xl size-28">
      <NuxtImg src="/avatar/me.jpg" alt="Alfredo Martínez" />
    </span>
  </div>
</template>

<script setup lang="ts">
defineOptions({
  name: 'Intro',
});
</script>
