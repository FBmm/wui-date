# wui-date

#### 项目介绍
基于angular.js的日期选择插件

#### 起步
1. 在你的项目引入wui.css或wui.min.css,以及font图标文件（与wui.css文件同级）
```html
<link rel="stylesheet" type="text/css" href="css/wui.min.css">
```
2. 在你的项目引入wui-date.js或wui-date.min.js,依赖angular.js
```html
<script type="text/javascript" src="js/angular.js" charset="utf-8"></script>
<script type="text/javascript" src="js/wui-date.js" charset="utf-8"></script>
```
3. 在你的项目引入wuiDate依赖
```js
var app = angular.module('app',["wui.date"]);
```
4. 在页面使用wui-date组件
```html
<wui-date 
    format="yyyy-mm-dd hh:mm:ss" 
    placeholder="请选择或输入日期" 
    id="date4" 
    btns="{'ok':'确定','now':'此刻'}" 
    ng-model="date4"
>
</wui-date>
```
#### 属性

>id：时间插件主键 , 默认：生成一个默认主键, 示例：id="date"

>name：input的name属性, 默认：空, 示例：name="date"

>format：定义时间格式, 默认：yyyy-mm-dd, 示例：format="yyyy-mm-dd hh:mm:ss"

>ng-model：$scope绑定的初始化以及选择后时间的属性, 默认：不能为空, >示例：ng-model="date"

>btns：定义底部按钮信息, 默认：空则隐藏所有按钮, 示例：btns="{'ok':'确定','now':'此刻','hitherto':true}" (ok表示确定按钮 now表示选择当前系统时间按钮 hitherto:true表示显示选择'至今'按钮)

>interval：定义time选择器时间间隔, 默认：30minutes, 示例：interval="20"

>position：选择框浮动位置, 默认：left, 示例：position="right"

>placeholder：选择框提示语 , 默认：选择时间, 示例：placeholder="请选择或输入日期"

>width：输入框宽度 支持px及百分比 , 默认：220px, 示例：width="220"或width="220px"或width="50%"

>size：选择插件内置大小 , 默认：小型, 示例：size="large"或size="L"

>dateClass：自定义插件class , 默认：无, 示例：dateClass="myDate"(css文件需添加.myDate {color: red;})
