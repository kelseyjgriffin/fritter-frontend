<!-- Page for profile info -->
<!-- User should be authenticated in order to see this page -->

<template>
  <main>
    <section>
      <header>
        <h2>Profile for {{ $store.state.username }}</h2>
        <h4 class="birthday">{{user.birthday}}</h4>
        <h4 class="bio">{{user.bio}}</h4>
      </header>
    </section>
    <section>
      <ProfileComponent />
    </section>
  </main>
</template>

<script>

export default {
  name: 'ProfilePage'
};
</script>