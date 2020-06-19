<template>
  <div class="column">
    <div class="card">
      <header class="card-header">
        <div class="content">
          <b-icon :icon="icon" type="is-primary" />
        </div>
        <p class="card-header-title has-text-grey">
          {{ title }}
        </p>
      </header>
      <div class="card-content">
        <figure class="image is-3by1">
          <img  v-bind:src="image" />
        </figure>
      </div>
      <cardFooter>

      </cardFooter>
    </div>
  </div>
</template>

<script>
import CardFooter from "~/components/CardFooter";
export default {
  props: {
    title: {
      type: String,
      required: true
    },

    image: {
      type: String,
      required: true
    },

    icon: {
      type: String,
      required: true
    }
  },
  components: {
    CardFooter
  }
};
</script>
