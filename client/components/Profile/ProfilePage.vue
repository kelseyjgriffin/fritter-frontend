<!-- Page for profile info -->
<!-- User should be authenticated in order to see this page -->

<template>
  <main>
    <section>
      <header>
        <h2>Profile for {{ $store.state.name }}</h2>
        <h3>Username: {{ $store.state.username }}</h3>
        <h3 v-if="$store.state.birthday">Birthday: {{ $store.state.birthday }}</h3>
        <h3 v-if="$store.state.bio">Bio: {{ $store.state.bio }}</h3>
      </header>
    </section>
    <section>
      <ProfileComponent/>
    </section>
  </main>
</template>

<script>
import ProfileComponent from '@/components/Profile/ProfileComponent.vue';

export default {
  name: 'ProfilePage',
  components: {
    ProfileComponent,
  }
};
</script>