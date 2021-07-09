<template>
  <div class="modal-backdrop" @click="$emit('close')">
    <div class="modal">
      <h3>Заголовок модального окна</h3>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
        tempor incididunt ut labore et dolore magna aliqua.
      </p>
    </div>
  </div>
</template>

<script>
export default {
  emits: ['close']
}
</script>

<style>
</style>
