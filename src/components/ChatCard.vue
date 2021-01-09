<template>
  <div class="flex w-full p-4" :class="{ 'bg-gray-600': active }">
    <div class="rounded-full w-10 h-10 bg-gray-300 mr-4"></div>
    <div>
      <h4 class="font-bold">{{ person.name }}</h4>
      <p class="text-white text-sm">{{ person.lastMessage }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "ChatCard",
  props: {
    person: Object,
    active: Boolean,
  },
};
</script>

<style lang="sass" scoped>
</style>