<!-- Page for profile info -->
<!-- User should be authenticated in order to see this page -->

<template>
  <main>
    <section>
      <header>
        <h2 class="profilename">Hi, My name is {{ $store.state.name }}</h2>
        <h3 class="profileusername"><mark>Username: {{ $store.state.username }}</mark></h3>
        <h3 class="profilebday" v-if="$store.state.birthday">Birthday: {{ $store.state.birthday }}</h3>
        <h3 class="profilebio" v-if="$store.state.bio">A bit about me: {{ $store.state.bio }}</h3>
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

<style scoped>
main {
  background-color: #CAE5FF;
  padding: 20px;
}

.profilename {
  color:#1B2845;
  text-align: center;
  font-size: 40px;
}

.profileusername {
  text-align: center;
  font-size: 20px;
}

mark{
  background-color: #B57BA6;
  color: white;
}

.profilebday {
  color:#274060;
  text-align: center;
  font-size: 30px;
}

.profilebio {
  color:#274060;
  text-align: center;
  font-size: 30px;
}
</style>