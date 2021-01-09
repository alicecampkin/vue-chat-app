<template>
  <form
    class="container max-w-screen-md bg-gray-200 my-4 shadow-md flex h-20 rounded"
  >
    <input
      type="text-area"
      name="message"
      id="message"
      class="h-full flex-grow bg-gray-200 text-gray-700 p-4"
      placeholder="Your message here..."
    />
    <input type="submit" value="Send" class="w-20 bg-green-600 font-bold" />
  </form>
</template>

<script>
export default {
  name: "AddMessage",
  components: {},
};
</script>

<style scoped>
</style>