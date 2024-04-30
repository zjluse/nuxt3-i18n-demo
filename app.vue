<template>
  <div>
    <div>
      <button @click="setLocale('en')">en</button> |
      <button @click="setLocale('fr')">fr</button>
    </div>
    <p>{{ $t('welcome') }}</p>
    <p>{{ text }}</p>
    <NuxtWelcome />
  </div>
</template>

<script setup>
const { t, setLocale } = useI18n();

const text = ref(t('welcome'))
</script>
