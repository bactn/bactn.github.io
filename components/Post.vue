<template>
  <div class="column">
    <div class="post">
      <header class="post-header">
        <div class="content">
          <div class="columns">
            <figure class="image is-48x48">
              <img class="is-rounded" v-bind:src="icon" />
            </figure>
            <div class="colum">
              <div class="post-header-category">
                {{ category }}
              </div>
              <span class="post-header-date has-text-grey">
                {{ date }} · 
              </span>
              <span class="post-header-time has-text-grey">
                {{ time }} minutes read
              </span>
            </div>
          </div>
        </div>
      </header>

      <div class="post-content">
        <figure class="image is-3by1">
          <img v-bind:src="banner" />
        </figure>
      </div>

      <postFooter> </postFooter>
    </div>
  </div>
</template>

<script>
import PostFooter from "~/components/PostFooter";
export default {
  props: {
    category: {
      type: String,
      required: true
    },

    banner: {
      type: String,
      required: true
    },

    icon: {
      type: String,
      required: true
    },
    date: {
      type: String,
      required: true
    },
    time: {
      type: String,
      required: true
    },
  },
  components: {
    PostFooter
  }
};
</script>
