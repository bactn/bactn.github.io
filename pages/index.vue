<template>
  <section class="section">
    <div class="hero is-mobile">
      <card
        title="Free"
        icon="github-circle"
      >
        Open source on <a href="https://github.com/buefy/buefy">
          GitHub
        </a>
      </card>

      <card
        title="Responsive"
        icon="cellphone-link"
        image="https://cdn-images-1.medium.com/focal/1600/480/51/40/1*1TcklZWGXaOW0GuRYkuZHQ.jpeg"
      >
        <b class="has-text-grey">
          Every
        </b> component is responsive
      </card>

      <card
        title="Modern"
        icon="alert-decagram"
        image="https://miro.medium.com/fit/c/1400/420/1*7sFmEX9u1AcddsP1ow7i0w.jpeg"
      >
        Built with <a href="https://vuejs.org/">
          Vue.js
        </a> and <a href="http://bulma.io/">
          Bulma
        </a>
      </card>

      <card
        title="Lightweight"
        icon="arrange-bring-to-front"
        image="https://cdn-images-1.medium.com/focal/1600/480/51/40/1*1TcklZWGXaOW0GuRYkuZHQ.jpeg"
      >
        No other internal dependency
      </card>
    </div>
  </section>
</template>

<script>
import Card from '~/components/Card'

export default {
  name: 'HomePage',

  components: {
    Card
  }
}
</script>
