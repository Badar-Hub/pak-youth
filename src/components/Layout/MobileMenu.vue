<template>
  <div class="mobile-menu">
    <q-drawer v-bind="$attrs" side="left" overlay behavior="mobile" bordered>
      <div class="sidebar">
        <div class="row">
          <img class="q-mx-auto" src="@/assets/logo.png" />
        </div>
        <div class="row">
          <nav class="q-my-auto">
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
        </div>
      </div>
    </q-drawer>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.mobile-menu {
  .custom-row {
    width: 100%;
  }
  ul {
    display: flex;
    flex-direction: column;
    align-items: baseline;
  }
  a {
    padding: 15px 0;
  }
}
</style>
