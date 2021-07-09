<template>
  <div class="container">
    <div class="card">
      <button class="btn primary" @click="modal = true">
        Открыть модальное окно
      </button>

      <teleport to="#modal">
        <app-modal v-if="modal" @close="modal = false"></app-modal>
      </teleport>
    </div>
  </div>
</template>

<script>
import AppModal from './components/AppModal.vue'

export default {
  data () {
    return {
      modal: false
    }
  },
  components: {
    AppModal
  }
}
</script>

<style>
</style>
