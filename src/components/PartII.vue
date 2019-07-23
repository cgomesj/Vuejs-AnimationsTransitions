<template>
  <div class="row">
    <div class="col-sm-8 mx-auto text-center">
      <h2 class="my-3 text-secondary">The Super Quiz</h2>
      <div class="card mt-4">
        <div class="card-header">{{ actualQuestion }}</div>
        <div class="card-body"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      tests: [
        {
          question: "How much is 5 + 9?",
          answer: "14"
        },
        {
          question: "How much is 10 + 6?",
          answer: "16"
        },
        {
          question: "How much is 1 + 4?",
          answer: "5"
        }
      ]
    };
  },
  computed: {
    actualQuestion() {
      return this.tests[0].question;
    }
  }
};
</script>

<style  scoped>
</style>