# Nicepage
![Image text](https://github.com/duzhen-cn/Nicepage/blob/master/index.jpg)
### [demo](http://nicezz.com/NicePage/index.html)<br>
### 基于强大的LAYUI框架,通过扩展nicePage.js实现JSON数据格式的自动表格分页和跳转功能,配置简单,上手速度快，兼容IE5+<br>
#### 引入js,css文件夹即可
```javascript
			//标准json格式 目前只支持[{a:b,c:d},{a:b,c:d}]

			var json=[{"id":"1","name":"Tom","age":"12"},{"id":"2","name":"Joy","age":"13"}]

			//nameList与widthList的数组长度要一致
			nameList//数组为表格列名,如['序号','姓名','年龄']
			widthList//数组为列名的宽度,如['100','200','100']
			
			/**
			 * 初始化设置nicepage组件
			 *------------------------------------------------------------
			 * 进行数据组装,与layui交互进行元素渲染
			 *-------------------------------------------------------------
			 * @param    {string}  table     table的div id
			 * @param    {string}  bar     底部分页的div id
			 * @param    {int}  limit     每页默认行数
			 * @param    {string}  color     底部分页的颜色
			 * @param    {array}  layout     底部分页的布局,具体可参考layui api
			 *
			 * @date     2018-10-19
			 * @author   Thomas.dz <hzdz163@163.com>
			 */
			//初始化
			$(function () {
				nicePage.setCfg({
					table: 'table',
					bar: 'pageBar',
					limit: 20,
					color: '#1E9FFF',
					layout: ['count', 'prev', 'page', 'next', 'limit', 'skip']
				});
			});
			//初始化完成
