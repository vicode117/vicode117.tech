<script setup lang="ts">
defineOptions({
  name: 'IndexPage',
})

const router = useRouter()
const { t } = useI18n()

const subjectList = [
  { name: 'home.interesting_technology', link: '/interesting_technology' },
  { name: 'home.work_issues', link: '/work_issues' },
  { name: 'home.learning', link: '/learning' },
]

const go = (name: string) => {
  router.push(`${name}`)
}
</script>

<template>
  <h1>Vicode117's Blog</h1>
  <hr>
  <h2 v-for="item in subjectList" :key="item.name" @click="go(item.link)">
    {{ t(item.name) }}
  </h2>
</template>

<route lang="yaml">
meta:
  layout: home
</route>
