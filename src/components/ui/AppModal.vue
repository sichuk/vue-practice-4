<template>
  <div class="modal-backdrop" @click.self="$emit('close')">
    <div class="modal">
      <h3 v-if="title"> {{ title }}</h3>
      <slot />
    </div>

  </div>
</template>

<script>
export default {
  emits: ['close'],
  props: {
    title: {
      type: String
    }
  }

}
</script>

<style scoped>

</style>