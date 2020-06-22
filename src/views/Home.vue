<template>
  <div class="home">
    <!-- <HelloWorld heading="Welcome to Your Vue.js App"/> -->
    <div class="inner text-center">
      <h1>atam's site</h1>
      <v-img
        :src="require('../assets/img/dummy01.png')"
        contain
        height="150"
        width="150"
        class="my-8 mx-auto rounded-circle"
      />
      <h2 class="mb-5">atam(_nd)</h2>
      <p>atam だったり atam_nd だったりします。</p>
      <p>ゲームしたりなんなりを発信するサイトです。</p>
      <p>とりあえず拠点として設置</p>
      <p>レイアウトは随時修正します。たぶん。</p>

      <v-card
        class="mx-auto my-10"
        max-width="600"
        width="90%"
        tile
      >
        <Twitter />
      </v-card>

      <v-card
        class="mx-auto my-10"
        max-width="600"
        width="90%"
        tile
      >
        <Update heading="更新予定一覧" />
      </v-card>
      
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import Twitter from '@/components/Twitter'
import Update from '@/components/Update'

export default {
  name: 'Home',
  components: {
    Twitter,
    Update
  },
  mounted() {
    // this.items.sort(function(a,b) {
    //   return a.sort - b.sort
    // })
  }
}
</script>