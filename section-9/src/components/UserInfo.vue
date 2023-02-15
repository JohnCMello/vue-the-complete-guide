<template>
  <section>
    <Card>
      <template #header>
        <h3>{{ fullName }}</h3>
        <base-badge :type="role" :caption="role.toUpperCase()"></base-badge>
      </template>
      <template v-slot:default>
        <p>{{ infoText }}</p>
      </template>
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
