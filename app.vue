<template>
  <div>
    <UHeader>
      <template #logo>
        <NuxtImg class="w-36" src="logo-solvedrubik.png" alt="Logo" />
      </template>
      <template #right>
        <UColorModeButton />
      </template>
    </UHeader>
    <UMain>
      <NuxtPage />
    </UMain>
  </div>
</template>
