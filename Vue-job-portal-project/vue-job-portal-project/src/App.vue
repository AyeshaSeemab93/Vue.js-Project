<script>
export default {
  data() {
    return {
      name: "Vue Jobs",
      status: "pendidsfdng",
    };
  },
};
</script>
<template>
  <h1>Vue Jobs</h1>
  <h2>{{ name }}</h2>
  <p v-if="status === 'active'">Vue Jobs are active</p>
  <p v-else-if="status === 'pending'">Jobs are pending</p>
  <p v-else>Vue jobs is inactive</p>
</template>
