<template>
  <button @click="$emit('toggle-add-task')"  :style="{ background: color }" class="btn">{{ text }}</button>
</template>

<script>

export default {
  name: 'Button',
  props: {
    text: String,
    color: String,
  },
  methods: {
    onClick() {
      console.log('Adding new tasks');
    }
  },
}
</script>
