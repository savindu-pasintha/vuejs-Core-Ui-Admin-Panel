<template >
  <div>
    <TransactionVue />
    <br />
    <DailyForexVue />
    <br />
    <SearchbarVue />
    <br />
    <CTable align="middle" class="mb-0 border" hover responsive>
      <CTableHead color="light">
        <CTableRow>
          <CTableHeaderCell>Payout Countries</CTableHeaderCell>
          <CTableHeaderCell> CCY</CTableHeaderCell>
          <CTableHeaderCell>QQ Cost Rate (Avg)</CTableHeaderCell>
          <CTableHeaderCell>Payout CCY (Lowest)</CTableHeaderCell>
          <CTableHeaderCell>Payout Partner Cost Rate</CTableHeaderCell>
          <CTableHeaderCell>QQ Offer rate</CTableHeaderCell>
          <CTableHeaderCell>Margin</CTableHeaderCell>
          <CTableHeaderCell>Consumers Rate</CTableHeaderCell>
          <CTableHeaderCell>Gain/Loss</CTableHeaderCell>
          <CTableHeaderCell>Margin</CTableHeaderCell>
          <CTableHeaderCell>Bussiness Rate</CTableHeaderCell>
          <CTableHeaderCell>Gain/Loss</CTableHeaderCell>
        </CTableRow>
      </CTableHead>
      <CTableBody>
        <CTableRow v-for="item in tableExample" :key="item.id">
          <CTableDataCell class="text-center">{{ item.pc }}</CTableDataCell>
          <CTableDataCell class="text-center">{{ item.cc }}</CTableDataCell>
          <CTableDataCell class="text-center">{{ item.qcr }}</CTableDataCell>
          <CTableDataCell class="text-center">{{ item.pcc }}</CTableDataCell>
          <CTableDataCell class="text-center">{{ item.qqor }}</CTableDataCell>
          <CTableDataCell class="text-center">{{ item.m }}</CTableDataCell>
          <CTableDataCell class="text-center">{{ item.cr }}</CTableDataCell>
          <CTableDataCell class="text-center">{{ item.gl }}</CTableDataCell>
          <CTableDataCell class="text-center">{{ item.m2 }}</CTableDataCell>
          <CTableDataCell class="text-center">{{ item.br }}</CTableDataCell>
          <CTableDataCell class="text-center">{{ item.gl2 }}</CTableDataCell>
          <CTableDataCell class="text-center">{{ item.gl2 }}</CTableDataCell>
        </CTableRow>
      </CTableBody>

      <CTableHead color="light">
        <CTableRow>
          <CTableHeaderCell></CTableHeaderCell>
          <CTableHeaderCell>OTHER </CTableHeaderCell>
          <CTableHeaderCell>CURRENCIES</CTableHeaderCell>
        </CTableRow>
      </CTableHead>
      <CTableBody>
        <CTableRow v-for="item in tableExampleOther" :key="item.id">
          <CTableDataCell class="text-center">{{ item.pc }}</CTableDataCell>
          <CTableDataCell class="text-center">{{ item.cc }}</CTableDataCell>
          <CTableDataCell class="text-center">{{ item.qcr }}</CTableDataCell>
          <CTableDataCell class="text-center">{{ item.pcc }}</CTableDataCell>
          <CTableDataCell class="text-center">{{ item.qqor }}</CTableDataCell>
          <CTableDataCell class="text-center">{{ item.m }}</CTableDataCell>
          <CTableDataCell class="text-center">{{ item.cr }}</CTableDataCell>
          <CTableDataCell class="text-center">{{ item.gl }}</CTableDataCell>
          <CTableDataCell class="text-center">{{ item.m2 }}</CTableDataCell>
          <CTableDataCell class="text-center">{{ item.br }}</CTableDataCell>
          <CTableDataCell class="text-center">{{ item.gl2 }}</CTableDataCell>
          <CTableDataCell class="text-center">{{ item.gl2 }}</CTableDataCell>
        </CTableRow>
      </CTableBody>
    </CTable>
  </div>
</template>

<script>
import TransactionVue from './dashboardForex/Transactions.vue'
import DailyForexVue from './dashboardForex/DailyForex.vue'
import SearchbarVue from './dashboardForex/Searchbar.vue'

export default {
  name: 'Dashboard',
  components: { TransactionVue, DailyForexVue, SearchbarVue },
  setup() {
    const tableExample = [
      {
        id: 1,
        pc: 'India',
        cc: 'INR',
        qcr: '4.1200',
        pcc: '74.2210',
        qqor: '17.8440',
        m: '+0.0110',
        cr: '17.8550',
        gl: '-1.0122',
        m2: '+0.0110',
        br: '17.8550',
        gl2: '-1.0122',
      },
      {
        id: 2,
        pc: 'India',
        cc: 'INR',
        qcr: '4.1200',
        pcc: '74.2210',
        qqor: '17.8440',
        m: '+0.0110',
        cr: '17.8550',
        gl: '-1.0122',
        m2: '+0.0110',
        br: '17.8550',
        gl2: '-1.0122',
      },
      {
        id: 3,
        pc: 'India',
        cc: 'INR',
        qcr: '4.1200',
        pcc: '74.2210',
        qqor: '17.8440',
        m: '+0.0110',
        cr: '17.8550',
        gl: '-1.0122',
        m2: '+0.0110',
        br: '17.8550',
        gl2: '-1.0122',
      },
    ]
    const tableExampleOther = [
      {
        id: 1,
        pc: 'India',
        cc: 'INR',
        qcr: '4.1200',
        pcc: '74.2210',
        qqor: '17.8440',
        m: '+0.0110',
        cr: '17.8550',
        gl: '-1.0122',
        m2: '+0.0110',
        br: '17.8550',
        gl2: '-1.0122',
      },
      {
        id: 2,
        pc: 'India',
        cc: 'INR',
        qcr: '4.1200',
        pcc: '74.2210',
        qqor: '17.8440',
        m: '+0.0110',
        cr: '17.8550',
        gl: '-1.0122',
        m2: '+0.0110',
        br: '17.8550',
        gl2: '-1.0122',
      },
    ]

    return {
      tableExample,
      tableExampleOther,
    }
  },
}
</script>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
