<template>
  <div class="flex my-4" :class="styles.row">
    <div
      class="max-w-sm py-3 pl-4 pr-14 rounded shadow-lg relative"
      :class="styles.container"
    >
      <p>{{ message.text }}</p>
      <small
        class="absolute bottom-1 right-0 text-gray-200 text-xs font-light px-2"
        >23:59</small
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

  computed: {
    isUser: function () {
      return this.message.id % 2 == 0;
    },
    styles: function () {
      return {
        row: this.isUser ? "justify-end" : "justify-start",
        container: this.isUser ? "bg-gray-600" : "bg-gray-700",
        datePosition: this.isUser ? "right-0" : "left-0",
        dateAlign: this.isUser ? "text-right" : "text-left",
      };
    },
  },
};
</script>

<style scoped>
</style>