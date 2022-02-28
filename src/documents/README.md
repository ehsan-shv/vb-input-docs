# Introduction and Installation

**Vue 3 input component.**

## Types

- text
- number
- password
- tel
- email
- search
- textarea

::: tip
Support Vue 3 and Nuxt 3 and type-safe.
:::

## Installation

```bash
npm i vb-input
```

## Import to component

```js
<template>
  <VBInput
    :type="'text'"
    placeholder="name"
    label="Your Name"
    v-model="name"
  />
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue';
import VBInput from 'vb-input';
export default defineComponent({
  components: {
    VBInput,
  },
  setup() {
    const name = ref('');

    return { name };
  },
});
</script>
```
