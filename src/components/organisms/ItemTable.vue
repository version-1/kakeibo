<template>
  <table class="item-table__container">
    <GridTable
      v-for="(item, index) in items"
      :key="index"
      :item="item"
      @clickDeleteItemButton="sendDeleteItemId"
    />
  </table>
</template>
<script>
import GridTable from '@/components/molecules/GridTable.vue'
export default {
  name: 'ItemTable',
  components: {
    GridTable
  },
  // props: {
  //   items: {
  //     type: Array,
  //     required: true
  //   }
  // },
  computed: {
    items () {
      return this.$store.state.items
    }
  },
  methods: {
    sendDeleteItemId (id) {
      this.$emit('clickDeleteItemButton', id)
    }
  }
}
</script>
<style scoped lang="scss">
.item-table {
  &__container {
    width: 100%;
  }
}

</style>
