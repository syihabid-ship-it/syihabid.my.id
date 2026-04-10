<script setup>
const title = 'syihabid.github.my.id'
const description = 'Starter landing page powered by Nuxt UI for syihabid.github.my.id'

useHead({
  meta: [
    { name: 'viewport', content: 'width=device-width, initial-scale=1' },
    { name: 'description', content: description }
  ],
  link: [
    { rel: 'icon', href: '/favicon.ico' }
  ],
  htmlAttrs: {
    lang: 'en'
  }
})

useSeoMeta({
  title,
  description,
  ogTitle: title,
  ogDescription: description,
  twitterCard: 'summary_large_image'
})
</script>

<template>
  <UApp>
    <UContainer class="min-h-screen flex items-center justify-center py-12">
      <UCard class="w-full max-w-4xl overflow-hidden">
        <div class="grid gap-10 p-8 md:p-12">
          <div class="space-y-4">
            <UBadge color="primary" variant="soft" size="lg">syihabid.github.my.id</UBadge>
            <h1 class="text-4xl md:text-6xl font-bold tracking-tight">
              Nuxt UI starter untuk personal brand yang clean dan modern.
            </h1>
            <p class="text-base md:text-lg text-muted-foreground max-w-2xl">
              Dibuat sebagai starter landing page untuk akun syihabid, dengan tampilan elegan,
              responsive, dan siap dikembangkan menjadi portfolio atau profil publik.
            </p>
          </div>

          <div class="flex flex-wrap gap-3">
            <UButton color="primary" size="lg" to="mailto:hello@syihabid.github.my.id">
              Contact
            </UButton>
            <UButton color="neutral" size="lg" variant="soft" to="#about">
              About
            </UButton>
          </div>

          <UCard id="about" variant="soft">
            <div class="grid gap-4 md:grid-cols-3">
              <div>
                <p class="text-sm text-muted-foreground">Focus</p>
                <p class="font-semibold">Enterprise, AML, .NET</p>
              </div>
              <div>
                <p class="text-sm text-muted-foreground">Stack</p>
                <p class="font-semibold">Nuxt UI / Bun / PostgreSQL</p>
              </div>
              <div>
                <p class="text-sm text-muted-foreground">Status</p>
                <p class="font-semibold">Ready to deploy</p>
              </div>
            </div>
          </UCard>
        </div>
      </UCard>
    </UContainer>
  </UApp>
</template>
