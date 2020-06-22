
<template>
  <v-card class="mx-auto">
    <v-card-title>
      <v-icon middle left color="#26c6da">mdi-twitter</v-icon>
    </v-card-title>
    <v-flex xs12>
      <Timeline
        :id="user_id" sourceType="profile"
        :options="{ tweetLimit: '1'
        }"/>
    </v-flex>
  </v-card>
</template>

<script>
import { Timeline } from "vue-tweet-embed";
export default {
  components: {
    Timeline
  },
  data() {
    return {
      user_id: "atam_nd"
    };
  }
};
</script>