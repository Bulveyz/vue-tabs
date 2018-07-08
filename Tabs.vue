<template>
    <div>
        <div class="tabs">
            <ul>
                <li v-for="tab in tabs" :class="{'is-active': tab.isActive}">
                    <a href="#" @click="changeTab(tab)">{{tab.name}}</a>
                </li>
            </ul>
        </div>
        <div class="tab-ditails">
            <slot></slot>
        </div>
    </div>
</template>

<script>
  export default {
    data() {
      return {
        tabs: []
      }
    },
    created() {
      this.tabs = this.$children;
    },
    methods: {
      changeTab(changeTab) {
        this.tabs.forEach(tab => {
          tab.isActive = (changeTab._uid == tab._uid)
        });
      }
    }
  }
</script>

<style scoped>

</style>