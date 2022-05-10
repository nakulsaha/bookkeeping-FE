<template>
  <div>
    <md-table v-model="users" :table-header-color="tableHeaderColor">
      <md-table-row slot="md-table-row" slot-scope="{ item }">
        <md-table-cell md-label=""></md-table-cell>
        <md-table-cell md-label="">{{ item.name }}</md-table-cell>
        <md-table-cell md-label="Jan">{{ item.jan }}</md-table-cell>
        <md-table-cell md-label="Fab">{{ item.feb }}</md-table-cell>
        <md-table-cell md-label="Mar">{{ item.mar }}</md-table-cell>
        <md-table-cell md-label="Apr">{{ item.apr }}</md-table-cell>
        <md-table-cell md-label="May">{{ item.may }}</md-table-cell>
        <md-table-cell md-label="Jun">{{ item.jun }}</md-table-cell>
        <md-table-cell md-label="Jul">{{ item.jul }}</md-table-cell>
        <md-table-cell md-label="Aug">{{ item.aug }}</md-table-cell>
        <md-table-cell md-label="Sep">{{ item.sep }}</md-table-cell>
        <md-table-cell md-label="Oct">{{ item.oct }}</md-table-cell>
        <md-table-cell md-label="Nov">{{ item.nov }}</md-table-cell>
        <md-table-cell md-label="Dec">{{ item.dec }}</md-table-cell>
      </md-table-row>
    </md-table>
  </div>
</template>

<script>
export default {
  name: "simple-table",
  props: {
    tableHeaderColor: {
      type: String,
      default: "",
    },
  },
  data() {
    return {
      selected: [],
      users: [
        {
          name: "Income",
          jan: "100",
          feb: "50",
          mar: "150",
          apr: "0",
          may: "800",
          jun: "50",
          jul: "100",
          aug: "0",
          sep: "0",
          oct: "0",
          nov: "0",
          dec: "0",
        },
        {
          name: "Cumulative income",
          jan: "100",
          feb: "150",
          mar: "300",
          apr: "1100",
          may: "1150",
          jun: "1250",
          jul: "1250",
          aug: "1250",
          sep: "1250",
          oct: "1250",
          nov: "1250",
          dec: "1250",
        },
        {
          name: "Cost",
          jan: "200",
          feb: "70",
          mar: "120",
          apr: "200",
          may: "300",
          jun: "50",
          jul: "50",
          aug: "0",
          sep: "0",
          oct: "0",
          nov: "0",
          dec: "0",
        },
        {
          name: "Cumulative Cost",
          jan: "200",
          feb: "270",
          mar: "390",
          apr: "590",
          may: "890",
          jun: "940",
          jul: "990",
          aug: "990",
          sep: "990",
          oct: "990",
          nov: "990",
          dec: "990",
        },
        {
          name: "Result",
          jan: "-100",
          feb: "-20",
          mar: "30",
          apr: "-200",
          may: "500",
          jun: "0",
          jul: "50",
          aug: "0",
          sep: "0",
          oct: "0",
          nov: "0",
          dec: "0",
        },
      ],
    };
  },
};
</script>
