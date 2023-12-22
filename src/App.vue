<script setup lang="ts">
import { css } from '../styled-system/css';
import { defineAsyncComponent } from 'vue';

const asyncComponent = defineAsyncComponent(() => import('./async-component.vue'));
</script>

<template>
  <div :class="css({ fontSize: '5xl', fontWeight: 'bold' })">Hello 🐼!</div>
  <component :is="asyncComponent"></component>
</template>
