## 计数器 counter

### 描述

用于展现计数器。

### 使用效果

<preview page="counter"/>

### 示例

```html
<import name="my-button" src="apex-ui/components/button/index"></import>
<template>
  <div class="wrap">
    <div class="counter">
      <text>counter1: {{number1}}</text>
      <text>counter2: {{number2}}</text>
    </div>
    <my-button ontap="start()">开始</my-button>
    <my-button ontap="pauseResume()">暂停/恢复</my-button>
    <my-button ontap="reset()">重置</my-button>
    <my-button ontap="update()">更新</my-button>
  </div>
</template>
<style lang="less">
  .wrap {
    flex-direction: column;
    padding: 20px;

    .counter {
      padding: 40px 0;
      flex-direction: column;

      text {
        font-size: 40px;
      }
    }
  }
</style>
<script>
    import prompt from '@system.prompt';
    import Counter from 'apex-ui/components/counter/index';

    export default {
        data() {
            return {
                number1: 0,
                number2: 0
            }
        },
        onInit() {
            const that = this;
            this.counter1 = new Counter(1, 1024, 0, 2, {
                printValue(value) {
                    that.number1 = value;
                }
            });
            this.counter1.start();

            this.counter2 = new Counter(0, 666, 0, 5, {
                printValue(value) {
                    that.number2 = value;
                }
            });
        },
        start() {
            this.counter2.start(() => {
                prompt.showToast({
                    message: '已完成'
                })
            })
        },
        reset() {
            this.counter2.reset()
        },
        update() {
            this.counter2.update(1314)
        },
        pauseResume() {
            this.counter2.pauseResume()
        },
    }
</script>
```

### API

#### 组件属性

| 属性                 | 类型     | 默认值 | 说明               |
| -------------------- | -------- | ------ | ------------------ |
| startVal             | Number   | -      | 起始值             |
| endVal               | Number   | -      | 结束值             |
| decimals             | Number   | 0      | 小数点位数         |
| duration             | Number   | 0      | 刷新时间           |
| options              | Object   | -      | 配置项             |
| options.useEasing    | Boolean  | true   | 是否开启过渡动画   |
| options.useGrouping  | Boolean  | true   | 是否分隔数值       |
| options.separator    | String   | -      | 分隔符             |
| options.decimal      | String   | -      | 小数点符号         |
| options.easingFn     | Function | -      | 自定义过渡动画     |
| options.formattingFn | Function | -      | 自定义格式化函数   |
| options.printValue   | Function | -      | 渲染组件的回调函数 |
