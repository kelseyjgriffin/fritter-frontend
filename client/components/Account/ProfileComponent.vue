<!-- Reusable component representing a single freet and its actions -->
<!-- We've tagged some elements with classes; consider writing CSS using those classes to style them... -->

<template>
  <article class="profile">
    <header>
      <h3 class="name">
        {{ user.name }}
      </h3>
      <div>
        <h4 class="birthday">
          {{user.birthday}}
        </h4>
        <h4 class="bio">
          {{user.bio}}
        </h4>
      </div>
    </header>
  </article>
</template>

<script>
export default {
  name: 'ProfileComponent',
  props: {
    // Data from the stored freet
    user: {
      type: Object,
      required: true
    }
  },
    }

</script>

<style scoped>
.bio {
    border: 1px solid #111;
    padding: 20px;
    position: relative;
}
</style>
