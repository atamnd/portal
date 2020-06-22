<template>
  <v-footer
    padless
  >
    <v-row
      justify="center"
      no-gutters
    >
      <!-- <v-btn
        v-for="link in links"
        :key="link"
        color="white"
        text
        rounded
        class="my-2"
      >
        {{ link }}
      </v-btn> -->
      <v-col
        class="teal lighten-2 py-4 text-center white--text"
        cols="12"
      >
        <p>
          &copy; 2020 {{this.nowYear()}}<strong>atam (_nd)</strong>
        </p>
      </v-col>
    </v-row>
  </v-footer>
</template>

<script>
  export default {
    data: () => ({
      links: [
        'Home',
        'About Us',
        'Team',
        'Services',
        'Blog',
        'Contact Us',
      ],
    }),
    mounted() {

    },
    methods: {
      nowYear() {
        let year = new Date().getFullYear();
        if(year != 2020) {
          return '- ' + year;
        }
      }
    }
  }
</script>