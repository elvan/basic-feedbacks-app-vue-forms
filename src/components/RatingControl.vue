<template>
  <ul>
    <li :class="{ active: modelValue === 'poor' }">
      <button type="button" @click="activate('poor')">Poor</button>
    </li>
    <li :class="{ active: modelValue === 'average' }">
      <button type="button" @click="activate('average')">Average</button>
    </li>
    <li :class="{ active: modelValue === 'great' }">
      <button type="button" @click="activate('great')">Great</button>
    </li>
  </ul>
</template>

<script>
export default {
  props: ['modelValue'],
  emits: ['update:modelValue'],
  methods: {
    activate(option) {
      this.$emit('update:modelValue', option);
    },
  },
};
</script>

<style scoped>
.active {
  border-color: #a00078;
}

.active button {
  color: #a00078;
}

ul {
  display: flex;
  margin: 0.5rem 0;
  padding: 0;
  list-style: none;
}

li {
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 0 1rem;
  padding: 1rem;
  border: 1px solid #ccc;
}

button {
  border: none;
  font: inherit;
  cursor: pointer;
  background-color: transparent;
}
</style>
