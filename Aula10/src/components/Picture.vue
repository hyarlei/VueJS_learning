
<template>
  <img :src="avatar" :alt="description" />
</template>

<script>
export default {
  name: "Picture",
  data() {
    return {
      avatar: "/img/favicon.ico",
      description: "icon vue",
    };
  },
};
</script>

