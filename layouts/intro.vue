<template>
  <div class="slidev-layout intro grid">
    <LayoutHeader />
    <CornerCurves class="absolute left-0 top-0 transform rotate-90" />
    <div class="flex flex-col justify-center text-center">
      <slot />
    </div>
    <AsGraphic
      type="zigzag"
      class="absolute top-20 -right-30"
    />
  </div>
</template>

<style>

.slidev-layout.intro h1:first-of-type {
  margin-top: 100px;
  @apply text-4xl leading-4 font-display font-extrabold text-primary;
}

.slidev-layout.intro h1 {
  @apply text-4xl leading-4 font-display font-extrabold text-primary;
}

.slidev-layout.intro h1 + p {
  margin-top: 20px;
  @apply opacity-60 -mt-1 text-2xl leading-20 ;
}

.slidev-layout.intro a {
  margin-top: 30px;
  @apply text-secondary-400 hover:text-secondary-500 dark:(text-white hover:text-gray-200);
}
</style>
