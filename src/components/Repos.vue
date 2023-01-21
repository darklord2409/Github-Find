<template>
  <div class="repos">
    <ReposItem v-for="repos in getRepostSort" :key="repos.id" :repos="repos"/>
  </div>
</template>

<script>
import ReposItem from "@/components/ReposItem.vue";
import { mapState, mapGetters } from "vuex";
export default {
  components: {
    ReposItem,
  },
  computed: {
    ...mapGetters(["getRepostSort"]),
  },
};
</script>

<style>
</style>