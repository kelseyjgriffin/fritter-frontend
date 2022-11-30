<!-- Page for profile info -->
<!-- User should be authenticated in order to see this page -->

<template>
  <main>
    <section>
      <header>
        <h2>Profile for {{ $store.state.username }}</h2>
      </header>
    </section>
    <section>
      <ProfileComponent />
    </section>
  </main>
</template>

