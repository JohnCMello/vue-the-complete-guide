<template>
  <div>
    <h2>Manage Goals Component</h2>
    <input type="text" ref="goal">
    <button @click="setGoal">Set Goal</button>
    <teleport to="body">
      <ErrorModal v-if="inputIsInvalid">
        <h2>Error</h2>
        <button @click="closeModal">Gotcha!</button>
      </ErrorModal>
    </teleport>
  </div>
</template>

<script>
import ErrorModal from './ErrorModal.vue'

export default {
  components: {
    ErrorModal
  },
  data() {
    return {
      inputIsInvalid: false
    }
  },
  methods: {
    setGoal() {
      const enteredValue = this.$refs.goal.value
      if (enteredValue === '') {
        this.inputIsInvalid = true
      }
    },
    closeModal() {
      this.inputIsInvalid = false
    }
  }
}
</script>
