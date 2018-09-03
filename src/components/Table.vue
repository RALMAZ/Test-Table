<template>
  <div>
    <table class="container">
    	<thead>
    		<tr>
    			<th><h1>ID</h1></th>
    			<th><h1>Чекбокс</h1></th>
    			<th><h1>Фрукт</h1></th>
    			<th><h1>Вес</h1></th>
    		</tr>
    	</thead>
    	<tbody>

        <tableCell
          v-for="(item, index) in items"
          :key="index"
          :item="item"
        ></tableCell>

    	</tbody>
    </table>
  </div>
</template>

<script>
import tableCell from "@/components/TableCell.vue";

export default {
  name: 'Table',
  props: {
    items: {
      type: Array | Object,
      required: true
    }
  },
  components: {
    tableCell
  }
}
</script>
