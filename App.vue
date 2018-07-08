<template>
  <div id="app">
    <tabs>
      <tab name="Home" :selected="true">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quos, repellendus.
      </tab>

      <tab name="About">
        Lorem ipsum dolor sit amet.
      </tab>

      <tab name="Support">
        Lorem ipsum dolor sit amet, consectetur.
      </tab>

      <tab name="Support">
        Lorem ipsum dolor sit amet, consectetur.
      </tab>
    </tabs>
  </div>
</template>

<script>
  import Tabs from './components/Tabs'
  import Tab from './components/Tab'
export default {
  components: {
    Tabs,
    Tab
  }
}
</script>

