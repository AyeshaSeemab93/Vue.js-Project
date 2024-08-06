<script>
export default {
  data() {
    return {
      name: "Vue Jobs",
      status: "active",
      tasks: ["Vue", "React", "Angular"],
      link: "https://www.google.com",
    };
  },

  methods: {
    toggleStatus() {
      this.status = this.status === "active" ? "pending" : "active";
    },
  },
};
</script>
<template>
  <h1>Vue Jobs</h1>
  <h2>{{ name }}</h2>
  <p v-if="status === 'active'">Vue Jobs are active</p>
  <p v-else-if="status === 'pending'">Jobs are pending</p>
  <p v-else>Vue jobs is inactive</p>
  <h3>Tasks:</h3>
  <ul>
    <li v-for="task in tasks" :key="task">{{ task }}</li>
  </ul>
  <a :href="link">Click for google</a>
  <br />
  <!-- <button v-on:click="toggleStatus">Change Status</button> -->
  <button @click="toggleStatus">Change Status</button>
  
</template>
