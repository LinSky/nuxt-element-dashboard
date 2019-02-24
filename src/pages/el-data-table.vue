<template>
  <div class="">
    <el-data-table v-bind="tableConfig"></el-data-table>
  </div>
</template>

<script>
export default {
  data() {
    return {
      tableConfig: {
        url: '/example/users',
        columns: [
          {
            type: 'selection'
          },
          {
            prop: '',
            label: '组件名称'
          },
          {
            prop: '',
            label: '分类'
          },
          {
            prop: '',
            label: '版本'
          },
          {
            prop: '',
            label: '开发语言'
          },
          {
            prop: '',
            label: '最后更新时间'
          },
          {
            prop: '',
            label: '状态'
          },
          {
            prop: '',
            label: '开发语言'
          }
        ],
        searchForm: [
          {
            $type: 'input',
            $id: 'name',
            label: '组件名称',
            $el: {
              placeholder: '请输入'
            }
          },
          {
            $type: 'select',
            $id: 'type',
            label: '分类',
            $el: {
              placeholder: '请选择'
            }
          },
          {
            $type: 'select',
            $id: 'status',
            label: '状态',
            $el: {
              placeholder: '请选择'
            }
          }
        ],
        headerButtons: [
          {
            text: '删除',
            type: 'danger'
          }
        ],
        extraButtons: [
          {
            text: '查看',
            type: 'danger'
          },
          {
            text: '编辑',
            type: 'danger'
          },
          {
            text: '下架',
            type: 'danger'
          }
        ]
      }
    }
  },
  methods: {}
}
</script>
<style lang="stylus">
.index {
  .home-img {
    width: 100%;
  }
}
</style>
