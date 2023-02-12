<script setup lang="ts">
defineOptions({
  name: 'IndexPage',
})

const router = useRouter()
const { t } = useI18n()

const subjectList = [
  { name: 'learning.mdn_learning', link: '/learning/mdn-learning' },
]

const go = (name: string) => {
  router.push(`${name}`)
}
</script>

<template>
  <h1>learning</h1>
  <hr>
  <h2 v-for="item in subjectList" :key="item.name" @click="go(item.link)">
    {{ t(item.name) }}
  </h2>
  <div>
    <button btn text-sm m="3 t8" @click="router.back()">
      {{ t('button.back') }}
    </button>
  </div>
</template>

<route lang="yaml">
meta:
  layout: default
</route>
