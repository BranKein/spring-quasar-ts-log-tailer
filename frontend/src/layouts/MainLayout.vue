<template>
  <q-layout view="hHh lpR fFf">
    <q-header elevated class="bg-primary text-white" height-hint="98">
      <q-toolbar>
        <q-toolbar-title class="text-h6 text-weight-bold">
          <q-avatar>
            <q-icon name="fas fa-align-left" />
          </q-avatar>
          LogTailer
        </q-toolbar-title>
      </q-toolbar>

      <q-tabs align="left">
        <q-route-tab to="/tail" label="Log" />
        <q-route-tab to="/setting" label="Setting" />
      </q-tabs>
    </q-header>

    <q-drawer show-if-above side="left" bordered>
      <!-- drawer content -->
    </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
export default {
  setup() {
    return {};
  },
};
</script>
