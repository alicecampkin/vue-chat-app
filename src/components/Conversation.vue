<template>
  <section
    class="container max-w-screen-sm mx-auto p-6 flex-grow overflow-y-scroll"
  >
    <message v-for="msg in messages" :key="msg.id" :message="msg" />
  </section>
</template>

<script>
import Message from "./Message.vue";

export default {
  name: "Conversation",
  components: {
    Message,
  },
  data: function () {
    return {
      messages: [
        {
          id: 1,
          text: "Hiya Ness, hows it going?",
        },
        {
          id: 2,
          text: "Alright Dave. What's occuring?",
        },
        {
          id: 3,
          text: "What you drinking?",
        },
        {
          id: 4,
          text: "Capri Sun.",
        },
        {
          id: 5,
          text: "Same.",
        },
      ],
    };
  },
};
</script>

<style scoped>
</style>