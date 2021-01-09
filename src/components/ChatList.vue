<template>
  <div class="w-80 py-8 shadow-lg bg-gray-800">
    <h1 class="text-2xl my-4 px-6 font-extrabold">Chats</h1>
    <ul>
      <chat-card
        v-for="user in users"
        :person="user"
        :key="user.id"
        :active="user.id == 3"
      />
    </ul>
  </div>
</template>

<script>
import ChatCard from "./ChatCard.vue";

export default {
  name: "ChatList",
  components: {
    ChatCard,
  },
  data: function () {
    return {
      users: [
        {
          id: 1,
          name: "Bob",
          lastMessage: "How's it going?",
        },
        {
          id: 2,
          name: "Liz",
          lastMessage: "Sounds great!",
        },
        {
          id: 3,
          name: "Grace",
          lastMessage: "Love it.",
        },
        {
          id: 4,
          name: "Max",
          lastMessage: "How have you been?",
        },
      ],
    };
  },
};
</script>

<style lang="sass" scoped>
</style>