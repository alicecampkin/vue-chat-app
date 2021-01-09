<template>
  <layout>
    <conversation />
    <add-message />
  </layout>
</template>

<script>
import Conversation from "./components/Conversation.vue";
import AddMessage from "./components/AddMessage.vue";
import Layout from "./components/Layout.vue";

export default {
  name: "App",
  components: {
    Conversation,
    AddMessage,
    Layout,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: white;
  background: #fafafa;
}
</style>
