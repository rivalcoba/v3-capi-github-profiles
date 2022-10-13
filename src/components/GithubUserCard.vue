<template>
  <div class="ui card">
    <div class="image">
      <a class="ui green ribbon label">Vue 2</a>
      <img :src="user.avatar_url" />
    </div>
    <div class="content">
      <a class="header">{{ user.name }}</a>
      <div class="meta">
        <span class="date">{{ user.created_at }}</span>
      </div>
      <div class="description">
        {{ user.bio }}
      </div>
    </div>
    <div class="extra content">
      <a>
        <i class="user icon"></i>
        {{ user.followers }}
      </a>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";
// const props = defineProps({
//   username: {
//     type: String,
//     required: true,
//     default: "No name",
//   },
// });

//
const user = ref({});
</script>
