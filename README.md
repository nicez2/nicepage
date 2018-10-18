# Nicepage
### [demo](http://nicezz.com/NicePage/index.html)<br>
#### /*只需设置如下内容即可*/
			//JSON格式为标准格式 
			var json=[{"date":"18日星期四","sunrise":"06:06","high":"高温 16.0℃","low":"低温 9.0℃","sunset":"17:20","aqi":41.0,"fx":"北风","fl":"3-4级","type":"晴","notice":"愿你拥有比阳光明媚的心情"}]
			nameList//数组为表格列名,如['序号','姓名','年龄']
			widthList//数组为列名的宽度,如['100','200','100']
			//通过下面两个方法填充数据
			nicePage.returnList(json);
			var htmlString = nicePage.returnHtml(nameList, widthList);
			nicePage.setCfg({
				dom: 'demo20',//指定html元素渲染
				limit: 20,//每页20行数据
				color: '#1E9FFF',//分页的颜色
				layout: ['count', 'prev', 'page', 'next', 'limit', 'refresh', 'skip']//需要显示的布局
			});
