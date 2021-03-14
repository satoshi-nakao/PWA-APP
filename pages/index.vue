<template>
  <v-row color="primary" justify="center" align="center">
    <v-col cols="12" sm="8" md="6">
    <v-card>
      　<v-card-title class="headline">
          ようこそこのサイトへ！
        </v-card-title>
        <v-card-text>
          <p>
            私のコードを載せてます。<a
              href="https://github.com/satoshi-nakao"
              target="_blank"
              rel="noopener noreferrer"
            >
              My GitHub
            </a>.
          </p>
          <p>
            学習用に作成しました。<a
              href="https://twitter.com/ksQcRkD1DNl98WE"
              target="_blank"
              rel="noopener noreferrer"
              
            >
              twitter
            </a>.
          </p>
          <p>
            街歩き、建築物の写真を載せてます。<a
              href="https://www.instagram.com/uzisubmachineguhand/"
              target="_blank"
              rel="noopener noreferrer"
              title="contribute"
            >
              instagram
            </a>.
          </p>
         <div class="container">
        <clock color="#38b508" bg="#fff" size="200px"></clock>
         </div>
         
        </v-card-text>
        <v-card-actions>
          <v-spacer />
          <v-btn
            color="primary"
            nuxt
            to="/inspire"
          >
            Continue
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>


export default {
  data(){
    return{
      drawer: false,
      items: [
        {name: 'Profile',to: '/profile'},
        {name: 'Skill',to: '/skill'},
        {name: 'Works', to: '/works'},
        {name: 'Want',to: '/want'}
      ],
      title: "My Page"
    }
  }
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 10vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  font-size: 40px;
}
</style>