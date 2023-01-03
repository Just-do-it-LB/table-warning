<template>
  <div>
    <t-table
      rowKey="index"
      :data="showData"
      :columns="columns"
      :table-layout="tableLayout"
      bordered
    >
    </t-table>
  </div>
</template>
<script lang="jsx">
const showData = [];

for (let i = 0; i < 3; i++) {
  showData.push({
    index: i + 1,
    applicant: ['贾明', '张三', '王芳'][i % 3],
    matters: [
      '宣传物料制作费用',
      'algolia 服务报销',
      '相关周边制作费',
      '激励奖品快递费',
    ][i % 4],
    createTime: [
      '2022-01-01',
      '2022-02-01',
      '2022-03-01',
      '2022-04-01',
      '2022-05-01',
    ][i % 4],
  });
}

export default {
  data() {
    return {
      tableLayout: 'fixed',
      showData,
      columns: [
        {
          colKey: 'applicant',
          title: '申请人',
          width: 100,
          foot: '-',
        },
        {
          colKey: 'matters',
          title: '申请事项',
          width: 150,
          foot: '-',
        },
        {
          colKey: 'createTime',
          title: '申请日期',
          width: 120,
          foot: '-',
        },
      ],
    };
  },
  methods: {
    rehandleClickOp(data) {
      console.log(data);
    },
  },
};
</script>
