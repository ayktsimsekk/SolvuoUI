<template>
  <a
    :id="idVal"
    :href="hrefVal"
    :class="classVal"
    :blank="blankVal"
    :title="titleVal"
  >
    {{ textVal }}
  </a>
</template>

<script>
export default {
  name: 'ATagComponent',
  props: {
    hrefVal: {
      type: String,
      required: true
    },
    textVal: {
      type: String,
      required: true
    },
    classVal: {
      type: String,
      required: true
    },
    blankVal: {
      type: String,
      required: true
    },
    titleVal: {
      type: String,
      required: true
    },
    idVal: {
      type: String,
      required: true
    }
  }
}
</script>
