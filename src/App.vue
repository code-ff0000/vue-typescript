<script setup lang="ts">
import TheHeader from "@/components/TheHeader.vue";
import EntryEditor from "./components/EntryEditor.vue";
import EntryCard from "@/components/EntryCard.vue";

import { reactive } from "vue";

import type User from "@/types/User";

const user: User = reactive({
  id: 1,
  username: "code-ff0000",
  settings: [],
});

console.log(user.username);
</script>

<template>
  <main class="container m-auto p-10">
    <TheHeader />
    <EntryEditor />
    <ul>
      <li>
        <EntryCard />
      </li>
    </ul>
  </main>
</template>
