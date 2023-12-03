
<script setup lang="ts">
const data = [
  {
    name: 'baban',
    expression: '* * * * 1',
    lastExecutionDate: '12-12-2023',
    nextExecutionDate: '12-12-2023',
  },
  {
    name: 'anan',
    expression: '* * * * 1',
    lastExecutionDate: '12-12-2023',
    nextExecutionDate: '12-12-2023',
  },
  {
    name: 'nenen',
    expression: '* * * * 1',
    lastExecutionDate: '12-12-2023',
    nextExecutionDate: '12-12-2023',
  },
];

const headers = [
  { key: 'name', title: 'Isim', align: 'center' },
  { key: 'expression', title: 'CRON', align: 'center' },
  { key: 'lastExecutionDate', title: 'Son tarih', align: 'center' },
  { key: 'nextExecutionDate', title: 'Sonraki tarih', align: 'center' },
];
</script>

<template>
  <div>This is list page</div>

  <div>
    <v-data-table :items="data" :headers="headers"></v-data-table>
  </div>
</template>