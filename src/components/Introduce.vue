<template>
  <section>
    <v-layout
      column
      wrap
      class="my-5"
    >
      <v-flex xs12 sm4 class="my-3">
        <div class="text-xs-center">
          <h2 class="headline">소개</h2>
          <br>
          <p v-for="(message, index) in messages" v-bind:key="index">{{ message }}</p>
        </div>
      </v-flex>
    </v-layout>
  </section>
</template>

<script>
export default {
  data() {
    return {
      messages: [
        '스터디의 공통 주제는 없습니다',
        '중요한 것은 개발자로서 성장하고 싶은 욕심인것 같습니다',
        '퇴근 후 혹은 주말에 부담없이 같이 스터디할 수 있는 모임을 지향하고 있습니다'
      ]
    }
  }
}
</script>
