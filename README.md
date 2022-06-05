# ShoppingCarBestImplementation
<body spellcheck="0" class="editMode htmledit_views">Android 购物车的最佳实现（通过ExpandableLis
合计、删除、商品数量的加减，为了方便测试又新增了刷新数据功能。<br>项目博客地址：https://blog.csdn.net/qq941263013/article/details/80901277
<br>个人博客地址：https://blog.csdn.net/qq941263013<br>GIF效果图：<br><img src="https://github.com/wangyang0313/ShoppingC
arBestImplementation/blob/master/app/gif.gif" _xhe_src="https://github.com/wangyang0313/ShoppingCarBestImplementation/bl
ob/master/app/gif.gif"><br><br>简单说明（详细描述见博客、源码）：<br>&nbsp; &nbsp; 1.页面布局文件：实际开发中，如果遇到ScrollView嵌
套ExpandableListView控件，可以使用自定义控件ExpandableListViewForScrollView解决ScrollView嵌套ExpandableListView，ExpandableLi
stView显示不全的问题。（地址：https://blog.csdn.net/qq941263013/article/details/80655909）<br>&nbsp; &nbsp; 2.初始化数据（含B
ean类）：在bean类的DatasBean中新增了isSelect_shop属性，用来判断店铺是否被选中；在GoodsBean中新增了isSelect属性，用来判断商品是否被
中。<br>&nbsp; &nbsp; 3.初始化ExpandableListView：使用的是ExpandableListView，所以adapter继承BaseExpandableListAdapter，并实
现其未实现的方法。<br>&nbsp; &nbsp; 4.初始化ExpandableListView的数据：初始化了ExpandableListView的数据，并保证数据刷新时，页面保持
当前位置。同时也使ExpandableListView的所有组展开，并点击无效果。</body>
