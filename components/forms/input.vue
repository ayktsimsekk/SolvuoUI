<template>
  <div>
    <input
      :type="inputType"
      :placeholder="inputPlaceholder"
      class="ant-input ant-input-lg"
      :name="inputName"
    />
  </div>
</template>

<script>
export default {
  name: 'InputComponent',
  props: {
    inputName: {
      type: String,
      required: true
    },
    inputPlaceholder: {
      type: String,
      required: true
    },
    inputType: {
      type: String,
      required: true
    }
  }
}
</script>
