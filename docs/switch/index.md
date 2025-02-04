# Switch

-   category: Components
-   family: DataEntry
-   chinese: 开关组件
-   type: 表单

---

开关组件

## 何时使用

开/关切换器切换单个设置选项的状态。开关控制器中的选项，以及它所在的状态，应该用伴随的内联标签显示清楚。开关选择器具有和单选按钮一样的视觉属性。使用文本 “开” 和 “关” 滑动切换已经过时了。使用这里显示的开关选择器代替。

## 如何使用

对于 checkChildren 和 unCheckedChildren 的自定义要考虑文字大小，因为 switch 的宽度有限，默认一个汉字大小。如果设置成多个字或者英文要注意宽度控制。

## FAQ

1.23 版本增加了 `autoWidth` API，我们推荐用户默认开启，同时在2.0里也会默认设置为true。开启后，原 `<Switch style={{display: 'block'}}>` 写法的用户可能会出现样式异常。

## API

### Switch

| 参数                | 说明                                                                                                                                             | 类型       | 默认值      | 版本支持 |
| ----------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- | -------- | -------- | ---- |
| checkedChildren   | 打开时的内容                                                                                                                                         | any      | -        |      |
| size              | switch的尺寸<br><br>**可选值**:<br>'medium'(正常大小)<br>'small'(缩小版大小)                                                                                  | Enum     | 'medium' |      |
| unCheckedChildren | 关闭时的内容                                                                                                                                         | any      | -        |      |
| onChange          | 开关状态改变是触发此事件<br><br>**签名**:<br>Function(checked: Boolean, e: Event) => void<br>**参数**:<br>_checked_: {Boolean} 是否为打开状态<br>_e_: {Event} DOM事件对象 | Function | () => {} |      |
| checked           | 开关当前的值(针对受控组件)                                                                                                                                 | Boolean  | -        |      |
| defaultChecked    | 开关默认值 (针对非受控组件)                                                                                                                                | Boolean  | false    |      |
| disabled          | 表示开关被禁用                                                                                                                                        | Boolean  | false    |      |
| loading           | loading                                                                                                                                        | Boolean  | false    |      |
| onClick           | 鼠标点击事件<br><br>**签名**:<br>Function(e: Event) => void<br>**参数**:<br>_e_: {Event} DOM事件对象                                                         | Function | -        |      |
| onKeyDown         | 键盘按键事件<br><br>**签名**:<br>Function(e: Event) => void<br>**参数**:<br>_e_: {Event} DOM事件对象                                                         | Function | -        |      |
| isPreview         | 是否为预览态                                                                                                                                         | Boolean  | false    |      |
| renderPreview     | 预览态模式下渲染的内容<br><br>**签名**:<br>Function(value: number) => void<br>**参数**:<br>_value_: {number} 评分值                                              | Function | -        |      |
| autoWidth         | 开启后宽度根据内容自适应                                                                                                                                   | Boolean  | false    | 1.23 |

## 无障碍键盘操作指南

| 按键    | 说明     |
| :---- | :----- |
| Enter | 切换选中状态 |
| SPACE | 切换选中状态 |
