<template>
  <div class="header row screen-center justify-between q-px-sm">
    <router-link to="/">
      <img src="@/assets/logo.png" alt="logo" />
    </router-link>
    <nav v-if="$q.screen.gt.xs" class="q-my-auto">
      <ul>
        <q-btn unelevated to="/" label="Home" />
        <q-btn unelevated to="/about" label="About" />
        <q-btn-dropdown unelevated label="Online Apply">
          <q-list>
            <q-item clickable v-close-popup @click="onItemClick">
              <q-item-section>
                <q-item-label>
                  <router-link to="/">Online Apply</router-link>
                </q-item-label>
              </q-item-section>
            </q-item>
          </q-list>
        </q-btn-dropdown>
        <q-btn unelevated to="/donation" label="Donation" />
        <q-btn unelevated to="/contact" label="Contact Us" />
      </ul>
    </nav>
    <nav class="q-my-auto" v-else>
      <q-icon name="menu" size="lg" />
    </nav>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.header {
  img {
    max-width: 90px;
    width: 100%;
  }
  nav {
    a {
      color: black;
      text-decoration: none;
      &:hover {
        text-decoration: underline;
      }
    }
  }
}
</style>
