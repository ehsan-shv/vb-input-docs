# Props

| props             | required | type                                                                           |
| ----------------- | :------: | :----------------------------------------------------------------------------- |
| type              |   true   | **String**['text', 'number', 'email', 'password', 'search', 'tel', 'textarea'] |
| id                |  false   | **String**                                                                     |
| modelValue        |  false   | **[String, Number]** (default: '')                                             |
| error             |  false   | **String** (default: false)                                                    |
| rtl               |  false   | **Boolean** (default: false)                                                   |
| label             |  false   | **String** (default: '')                                                       |
| labelInline       |  false   | **Boolean** (default: false)                                                   |
| blockStyle        |  false   | **Object** (default: {})                                                       |
| fieldStyle        |  false   | **Object** (default: {})                                                       |
| errorMessageStyle |  false   | **Object** (default: {})                                                       |
| labelStyle        |  false   | **Object** (default: {})                                                       |
| buttonStyle       |  false   | **Object** (default: {})                                                       |
| buttonText        |  false   | **String** (default: '')                                                       |
| hasButton         |  false   | **Boolea** (default: false)                                                    |

::: tip
You can bind other input attributes(disabled, aoutofocus, max, min, ...) like normal input tag.
:::

```js
<template>
  <VBInput
    :type="'text'"
    placeholder="name"
    disabled
    autofocus
  />
</template>
```
