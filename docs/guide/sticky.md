## 吸顶容器 sticky

### 描述

用于在滚动页面时将标题栏固定在顶部

### 使用效果

<preview page="sticky"/>

### 使用方法

在`.ux`文件中引入组件

```html
<import name="my-sticky" src="apex-ui/components/sticky/index.ux"></import>
<import name="my-sticky-item" src="apex-ui/components/sticky-item/index.ux"></import>
```

### 示例

```html
<template>
  <div>
    <my-sticky id="sticky1">
      <my-sticky-item group-id="sticky1" title="🐶🐶🐶🐶">
        <div class="my-content" slot="content">
          <div class="demo-item"><text>呦呦呦呦呦呦呦呦呦呦呦呦</text></div>
          <div class="demo-item"><text>啦啦啦啦啦啦啦啦啦啦</text></div>
          <div class="demo-item"><text>哔卟哔卟哔卟哔卟哔卟哔卟哔卟</text></div>
          <div class="demo-item"><text>略略略略略略略略略略略略略略略略</text></div>
          <div class="demo-item"><text>嘎嘎嘎嘎嘎嘎嘎嘎嘎嘎</text></div>
          <div class="demo-item"><text>吱吱喳喳吱吱喳喳</text></div>
          <div class="demo-item"><text>哗啦啦哗啦啦哗啦啦哗啦啦哗啦啦哗啦啦</text></div>
          <div class="demo-item"><text>红红火火恍恍惚惚红红火火恍恍惚惚</text></div>
        </div>
      </my-sticky-item>
      <my-sticky-item group-id="sticky1" title="🐱🐱🐱🐱">
        <div class="my-content" slot="content">
          <div class="demo-item"><text>呦呦呦呦呦呦呦呦呦呦呦呦</text></div>
          <div class="demo-item"><text>啦啦啦啦啦啦啦啦啦啦</text></div>
          <div class="demo-item"><text>哔卟哔卟哔卟哔卟哔卟哔卟哔卟</text></div>
          <div class="demo-item"><text>略略略略略略略略略略略略略略略略</text></div>
          <div class="demo-item"><text>嘎嘎嘎嘎嘎嘎嘎嘎嘎嘎</text></div>
          <div class="demo-item"><text>吱吱喳喳吱吱喳喳</text></div>
          <div class="demo-item"><text>吱吱喳喳吱吱喳喳</text></div>
          <div class="demo-item"><text>红红火火恍恍惚惚红红火火恍恍惚惚</text></div>
          <div class="demo-item"><text>哗啦啦哗啦啦哗啦啦哗啦啦哗啦啦哗啦啦</text></div>
          <div class="demo-item"><text>红红火火恍恍惚惚红红火火恍恍惚惚</text></div>
        </div>
      </my-sticky-item>
      <my-sticky-item group-id="sticky1" title="🐭🐭🐭🐭">
        <div class="my-content" slot="content">
          <div class="demo-item"><text>呦呦呦呦呦呦呦呦呦呦呦呦</text></div>
          <div class="demo-item"><text>啦啦啦啦啦啦啦啦啦啦</text></div>
          <div class="demo-item"><text>哔卟哔卟哔卟哔卟哔卟哔卟哔卟</text></div>
          <div class="demo-item"><text>略略略略略略略略略略略略略略略略</text></div>
          <div class="demo-item"><text>嘎嘎嘎嘎嘎嘎嘎嘎嘎嘎</text></div>
          <div class="demo-item"><text>吱吱喳喳吱吱喳喳</text></div>
          <div class="demo-item"><text>吱吱喳喳吱吱喳喳</text></div>
          <div class="demo-item"><text>红红火火恍恍惚惚红红火火恍恍惚惚</text></div>
          <div class="demo-item"><text>哗啦啦哗啦啦哗啦啦哗啦啦哗啦啦哗啦啦</text></div>
          <div class="demo-item"><text>红红火火恍恍惚惚红红火火恍恍惚惚</text></div>
        </div>
      </my-sticky-item>
      <my-sticky-item group-id="sticky1" title="🐹🐹🐹🐹">
        <div class="my-content" slot="content">
          <div class="demo-item"><text>呦呦呦呦呦呦呦呦呦呦呦呦</text></div>
          <div class="demo-item"><text>啦啦啦啦啦啦啦啦啦啦</text></div>
          <div class="demo-item"><text>哔卟哔卟哔卟哔卟哔卟哔卟哔卟</text></div>
          <div class="demo-item"><text>略略略略略略略略略略略略略略略略</text></div>
          <div class="demo-item"><text>嘎嘎嘎嘎嘎嘎嘎嘎嘎嘎</text></div>
          <div class="demo-item"><text>吱吱喳喳吱吱喳喳</text></div>
          <div class="demo-item"><text>哗啦啦哗啦啦哗啦啦哗啦啦哗啦啦哗啦啦</text></div>
          <div class="demo-item"><text>红红火火恍恍惚惚红红火火恍恍惚惚</text></div>
        </div>
      </my-sticky-item>
      <my-sticky-item group-id="sticky1" title="🐸🐸🐸🐸">
        <div class="my-content" slot="content">
          <div class="demo-item"><text>呦呦呦呦呦呦呦呦呦呦呦呦</text></div>
          <div class="demo-item"><text>啦啦啦啦啦啦啦啦啦啦</text></div>
          <div class="demo-item"><text>哔卟哔卟哔卟哔卟哔卟哔卟哔卟</text></div>
          <div class="demo-item"><text>红红火火恍恍惚惚红红火火恍恍惚惚</text></div>
          <div class="demo-item"><text>略略略略略略略略略略略略略略略略</text></div>
          <div class="demo-item"><text>嘎嘎嘎嘎嘎嘎嘎嘎嘎嘎</text></div>
          <div class="demo-item"><text>吱吱喳喳吱吱喳喳</text></div>
          <div class="demo-item"><text>红红火火恍恍惚惚红红火火恍恍惚惚</text></div>
          <div class="demo-item"><text>哗啦啦哗啦啦哗啦啦哗啦啦哗啦啦哗啦啦</text></div>
          <div class="demo-item"><text>红红火火恍恍惚惚红红火火恍恍惚惚</text></div>
        </div>
      </my-sticky-item>
      <my-sticky-item group-id="sticky1" title="🥺🥺🥺🥺">
        <div class="my-content" slot="content">
          <div class="demo-item"><text>呦呦呦呦呦呦呦呦呦呦呦呦</text></div>
          <div class="demo-item"><text>啦啦啦啦啦啦啦啦啦啦</text></div>
          <div class="demo-item"><text>哔卟哔卟哔卟哔卟哔卟哔卟哔卟</text></div>
          <div class="demo-item"><text>略略略略略略略略略略略略略略略略</text></div>
          <div class="demo-item"><text>嘎嘎嘎嘎嘎嘎嘎嘎嘎嘎</text></div>
          <div class="demo-item"><text>吱吱喳喳吱吱喳喳</text></div>
          <div class="demo-item"><text>红红火火恍恍惚惚红红火火恍恍惚惚</text></div>
          <div class="demo-item"><text>哗啦啦哗啦啦哗啦啦哗啦啦哗啦啦哗啦啦</text></div>
          <div class="demo-item"><text>红红火火恍恍惚惚红红火火恍恍惚惚</text></div>
        </div>
      </my-sticky-item>
      <my-sticky-item group-id="sticky1" title="🤩🤩🤩🤩">
        <div class="my-content" slot="content">
          <div class="demo-item"><text>呦呦呦呦呦呦呦呦呦呦呦呦</text></div>
          <div class="demo-item"><text>啦啦啦啦啦啦啦啦啦啦</text></div>
          <div class="demo-item"><text>哔卟哔卟哔卟哔卟哔卟哔卟哔卟</text></div>
          <div class="demo-item"><text>略略略略略略略略略略略略略略略略</text></div>
          <div class="demo-item"><text>嘎嘎嘎嘎嘎嘎嘎嘎嘎嘎</text></div>
          <div class="demo-item"><text>红红火火恍恍惚惚红红火火恍恍惚惚</text></div>
          <div class="demo-item"><text>吱吱喳喳吱吱喳喳</text></div>
          <div class="demo-item"><text>哗啦啦哗啦啦哗啦啦哗啦啦哗啦啦哗啦啦</text></div>
          <div class="demo-item"><text>红红火火恍恍惚惚红红火火恍恍惚惚</text></div>
        </div>
      </my-sticky-item>
      <my-sticky-item group-id="sticky1" title="🤯🤯🤯🤯">
        <div class="my-content" slot="content">
          <div class="demo-item"><text>呦呦呦呦呦呦呦呦呦呦呦呦</text></div>
          <div class="demo-item"><text>啦啦啦啦啦啦啦啦啦啦</text></div>
          <div class="demo-item"><text>哔卟哔卟哔卟哔卟哔卟哔卟哔卟</text></div>
          <div class="demo-item"><text>略略略略略略略略略略略略略略略略</text></div>
          <div class="demo-item"><text>嘎嘎嘎嘎嘎嘎嘎嘎嘎嘎</text></div>
          <div class="demo-item"><text>吱吱喳喳吱吱喳喳</text></div>
          <div class="demo-item"><text>吱吱喳喳吱吱喳喳</text></div>
          <div class="demo-item"><text>红红火火恍恍惚惚红红火火恍恍惚惚</text></div>
          <div class="demo-item"><text>哗啦啦哗啦啦哗啦啦哗啦啦哗啦啦哗啦啦</text></div>
          <div class="demo-item"><text>红红火火恍恍惚惚红红火火恍恍惚惚</text></div>
        </div>
      </my-sticky-item>
      <my-sticky-item group-id="sticky1" title="🤔🤔🤔🤔">
        <div class="my-content" slot="content">
          <div class="demo-item"><text>呦呦呦呦呦呦呦呦呦呦呦呦</text></div>
          <div class="demo-item"><text>啦啦啦啦啦啦啦啦啦啦</text></div>
          <div class="demo-item"><text>哔卟哔卟哔卟哔卟哔卟哔卟哔卟</text></div>
          <div class="demo-item"><text>略略略略略略略略略略略略略略略略</text></div>
          <div class="demo-item"><text>嘎嘎嘎嘎嘎嘎嘎嘎嘎嘎</text></div>
          <div class="demo-item"><text>吱吱喳喳吱吱喳喳</text></div>
          <div class="demo-item"><text>吱吱喳喳吱吱喳喳</text></div>
          <div class="demo-item"><text>红红火火恍恍惚惚红红火火恍恍惚惚</text></div>
          <div class="demo-item"><text>哗啦啦哗啦啦哗啦啦哗啦啦哗啦啦哗啦啦</text></div>
          <div class="demo-item"><text>红红火火恍恍惚惚红红火火恍恍惚惚</text></div>
        </div>
      </my-sticky-item>
    </my-sticky>
  </div>
</template>
```

```less
<style>
.my-content {
  flex-direction: column;
  background-color: #fff;
  width: 100%;
}

.demo-item {
  border-bottom: 1px solid #ddd;
  padding: 20px;
}

text {
  color: #000;
}
</style>
```

### API

#### sticky组件属性

| 属性 | 类型    | 默认值 | 说明              |
| ---- | ------ | ----- | ---------------- |
| id   | String | ''    | sticky组件ID，必填 |

#### sticky-item组件属性

| 属性    | 类型    | 默认值 | 说明                 |
| ------- | ------ | ----- | ------------------- |
| title   | String | '' | 标题                    |
| content | String | '' | 内容                    |
| groupId | String | '' | 所属的sticky组件的ID，必填 |

#### sticky-item slot

| 名称    |描述       | 
| ------- | -------- | 
| content | 自定义标题 |