<template>
  <div class="flex my-10">
    <div class="max-w-sm p-4 bg-gray-700 rounded shadow-lg relative">
      <p>{{ message.text }}</p>
      <small class="w-40 absolute -bottom-6 text-gray-600"
        >45 minutes ago</small
      >
    </div>
  </div>
</template>

<script>
export default {
  name: "Message",
  props: {
    message: Object,
  },
};
</script>

<style scoped>
</style>