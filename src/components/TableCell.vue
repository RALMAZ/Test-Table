<template>
    <tr :class="{ 'redhead': item.selected }">
    	<td v-text="item.id"></td>
    	<td><Checkbox :item="item"></Checkbox></td>
    	<td v-if="!item.selected" v-text="item.title"></td>
        <td v-else>-</td>
    	<td v-if="!item.selected" v-text="item.weight"></td>
        <td v-else>-</td>
    </tr>
</template>

<script>
import Checkbox from "@/components/Checkbox.vue";

export default {
  name: 'TableCell',
  props: {
    item: {
        type: Array | Object,
        required: true
    }
  },
  components: {
    Checkbox
  }
}
</script>

<style>
.redhead {
    background-color: #8a2424 !important;
}
</style>

