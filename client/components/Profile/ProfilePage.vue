<!-- Page for profile info -->
<!-- User should be authenticated in order to see this page -->

<template>
  <main>
    <section>
      <header>
        <h2>Profile for {{ $store.state.username }}</h2>
        <h3>Name:{{ $store.state.name }}</h3>
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