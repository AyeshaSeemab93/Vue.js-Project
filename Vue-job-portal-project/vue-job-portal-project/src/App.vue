<script setup>
import NavBar from "@/components/Navbar.vue";
import Hero from "@/components/Hero.vue";
import HomeCards from "@/components/HomeCards.vue";
import JobListings from "@/components/JobListings.vue";
</script>
<template>
  <NavBar />
  <Hero title="Test Title" />
  <HomeCards />
  <JobListings :limit="4" showButton="true" />
</template>
