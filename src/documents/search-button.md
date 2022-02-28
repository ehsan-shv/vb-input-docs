# Search Button

```js
<template>
  <VBInput
    :type="'search'"
    :hasButton="true"
    @onInputButtonClick="onInputButtonClick"
  />
</template>
```

::: tip
Serch input has an icon by default. You can customize by changing **background-image** in CSS.
:::

::: warning
Serch button just emit an event to parent.
:::
