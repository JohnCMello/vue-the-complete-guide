<template>
  <section>
    <Card>
      <header>
        <h3>{{ fullName }}</h3>
        <base-badge :type="role" :caption="role.toUpperCase()"></base-badge>
      </header>
      <p>{{ infoText }}</p>
    </Card>
  </section>
</template>

<script>
import Card from './Card.vue';

export default {
  props: ['fullName', 'infoText', 'role'],
  components: { Card },
};
</script>

<style scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
</style>
