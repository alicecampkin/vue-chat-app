<template>
  <div class="h-screen flex">
    <chat-list />
    <main class="container flex flex-col flex-grow justify-between bg-gray-300">
      <conversation-header />
      <slot />
    </main>
  </div>
</template>

<script>
import ChatList from "./ChatList.vue";
import ConversationHeader from "./ConversationHeader.vue";

export default {
  name: "Layout",
  components: {
    ChatList,
    ConversationHeader,
  },
};
</script>

<style lang="sass" scoped>
</style>