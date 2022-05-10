<template>
  <div class="content">
    <p>Chose Year</p>
			<select v-model="selectedOption">
				<option v-for="fruit in fruitArray" v-bind:key="fruit.Id" v-bind:value="fruit.id">{{ fruit.Name }}</option>
			</select>
    <div class="md-layout">
      <div
        class="md-layout-item md-medium-size-100 md-xsmall-size-100 md-size-100"
      >
        <md-card>
          <md-card-header data-background-color="green">
            <h4 class="title">Year {{selectedOption}}</h4>
          </md-card-header>
          <md-card-content>
            <simple-table table-header-color="green"></simple-table>
          </md-card-content>
        </md-card>
      </div>

      <div
        class="md-layout-item md-medium-size-100 md-xsmall-size-100 md-size-100"
      >
        <md-card class="md-card-plain">
          <md-card-header data-background-color="green">
            <h4 class="title">reconciliation</h4>
          </md-card-header>
          <md-card-content>
            <ordered-table></ordered-table>
          </md-card-content>
        </md-card>
      </div>
    </div>
  </div>
</template>

<script>
import { SimpleTable, OrderedTable } from "@/components";

export default {
  components: {
    OrderedTable,
    SimpleTable,
  },
  data() {
    return {
      selectedOption : 2019, 
      fruitArray: [{id: 2019, 'Name': '2019'},{id: 2020, 'Name': '2020'}],
    }
  }
};
</script>

<style scoped>
  h4{
    align-content: center
  }
</style>