# Event Emitter

You can emit an event to parent component.

```js
<template>
  <VBInput
    @onInputButtonClick="onInputButtonClick"
    :type="'text'"
    placeholder="name"
    label="Your Name"
    v-model="name"
    :hasButton="true"
    :buttonText="'send'"
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

    const onInputButtonClick = () => {
      console.log('Event emitted...');
    };

    return { onInputButtonClick, name };
  },
});
</script>
```

::: tip
**@onInputButtonClick** doesn't pass any data.
:::

::: warning
When you need emit an event to parent you should set **hasButton** prop to **true**.
:::
