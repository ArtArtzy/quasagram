<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated>
      <q-toolbar>
        <q-btn
          flat
          dense
          round
          icon="menu"
          aria-label="Menu"
          @click="leftDrawerOpen = !leftDrawerOpen"
        />

        <q-toolbar-title>
          Quasar App
        </q-toolbar-title>


      </q-toolbar>
    </q-header>

  <q-footer class="bg-white" bordered >
    <q-tabs class="text-grey-10" active-color="primary" indicator-color="transparent"  >
      <q-route-tab name="mails" icon="mail" label="Home" to="/" />
      <q-route-tab name="alarms" icon="alarm" label="Camera" to="camera" />
    </q-tabs>
  </q-footer>


    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>


export default {
  name: 'MainLayout',
  data () {
    return {
      
    }
  }
}
</script>
