# SplitButton

-   category: Components
-   family: General
-   chinese: 分隔按钮
-   type: 基本

---

由两部分组成的按钮，左侧触发操作，右侧触发菜单。

## 何时使用

-   `SplitButton` 由 `Button` 和 `Menu` 组成，右侧 `Icon` 按钮部分为弹层菜单的触发区域，存放多个操作，左侧按钮部分则进行操作触发；
-   推荐按钮操作多于3种时使用。

## API

### SplitButton

| 参数                  | 说明                                                                                                                                                                                                                                        | 类型        | 默认值       |
| ------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- | --------- |
| size                | 按钮组的尺寸<br><br>**可选值**:<br>'small', 'medium', 'large'                                                                                                                                                                                      | Enum      | 'medium'  |
| type                | 按钮的类型<br><br>**可选值**:<br>'normal', 'primary', 'secondary'                                                                                                                                                                                 | Enum      | 'normal'  |
| label               | 主按钮的文案                                                                                                                                                                                                                                    | ReactNode | -         |
| component           | 设置标签类型<br><br>**可选值**:<br>'button', 'a'                                                                                                                                                                                                   | Enum      | -         |
| ghost               | 是否为幽灵按钮<br><br>**可选值**:<br>'light', 'dark', false, true                                                                                                                                                                                   | Enum      | -         |
| defaultSelectedKeys | 默认激活的菜单项（用法同 Menu 非受控）                                                                                                                                                                                                                    | Array     | \[]       |
| selectedKeys        | 激活的菜单项（用法同 Menu 受控）                                                                                                                                                                                                                       | Array     | -         |
| selectMode          | 菜单的选择模式<br><br>**可选值**:<br>'single', 'multiple'                                                                                                                                                                                           | Enum      | -         |
| onSelect            | 选择菜单项时的回调，参考 Menu<br><br>**签名**:<br>Function() => void                                                                                                                                                                                    | Function  | func.noop |
| onItemClick         | 点击菜单项时的回调，参考 Menu<br><br>**签名**:<br>Function() => void                                                                                                                                                                                    | Function  | func.noop |
| triggerProps        | 触发按钮的属性（支持 Button 的所有属性透传）                                                                                                                                                                                                                | Object    | -         |
| autoWidth           | 弹层菜单的宽度是否与按钮组一致                                                                                                                                                                                                                           | Boolean   | true      |
| visible             | 弹层是否显示                                                                                                                                                                                                                                    | Boolean   | -         |
| defaultVisible      | 弹层默认是否显示                                                                                                                                                                                                                                  | Boolean   | -         |
| onVisibleChange     | 弹层显示状态变化时的回调函数<br><br>**签名**:<br>Function(visible: Boolean, type: String) => void<br>**参数**:<br>_visible_: {Boolean} 弹层显示状态<br>_type_: {String} 触发弹层显示或隐藏的来源 menuSelect 表示由menu触发； fromTrigger 表示由trigger的点击触发； docClick 表示由document的点击触发 | Function  | func.noop |
| popupTriggerType    | 弹层的触发方式<br><br>**可选值**:<br>'click', 'hover'                                                                                                                                                                                               | Enum      | 'click'   |
| popupAlign          | 弹层对齐方式, 详情见Overlay align                                                                                                                                                                                                                  | String    | -         |
| popupStyle          | 弹层自定义样式                                                                                                                                                                                                                                   | Object    | -         |
| popupClassName      | 弹层自定义样式类                                                                                                                                                                                                                                  | String    | -         |
| popupProps          | 透传给弹层的属性                                                                                                                                                                                                                                  | Object    | -         |
| popupContainer      | 弹层容器                                                                                                                                                                                                                                      | any       | -         |
| followTrigger       | 是否跟随滚动                                                                                                                                                                                                                                    | Boolean   | -         |
| menuProps           | 透传给 Menu 的属性                                                                                                                                                                                                                              | Object    | {}        |
| leftButtonProps     | 透传给 左侧按钮 的属性                                                                                                                                                                                                                              | Object    | {}        |
