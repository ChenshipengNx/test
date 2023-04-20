## 表格控件
控件对象：com.kingdee.bos.ctrl.kdf.table.KDTable
### 视觉展示
![](/media/202108/2021-08-30_094402.png)
### 常用属性
| 字段通用属性 | 属性ID | 类型     | 默认值 | 说明   |
|--------|------|--------|-----|------|
| 提示     | toolTipText | String |     | 设置移入提示|
| 可见性     | visible | boolean   |   true  | 设置控件可见 |

### 事件监听接口
| 监听接口                   | 方法名            | 说明        |
|------------------------|----------------|-----------|
| KDTMouseListener | tableClicked | 鼠标事件监听 |
| KDTEditAdapter | editStopped等 | 编辑事件 |
### 代码示例
#### 增加（删除）行或列
```java
//在指定位置插入列
kdtEntry.addColumn(colIndex);
//在最后一列插入
kdtEntry.addColumn();
//插入多列
kdtEntry.addColumns(colCount);
//删除列
kdtEntry.removeColumn(index);
```
#### 增加（删除）表头
```java
//增加表头行
kdtEntry.addHeadRow(rowIndex);
//增加到最后
kdtEntry.addHeadRow();
//删除所有表头行
kdtEntry.removeHeadRows();
```
#### 增加（删除）表体行
```java
//指定位置插入
kdtEntry.addRow(rowIndex);
//插入到最后
kdtEntry.addRow();
//删除指定行
kdtEntry.removeRow(rowIndex);
//删除所有行
kdtEntry.removeRows();
```
#### 获取列、行、单元格对象
```java
//获取列对象
IColumn column = kdtEntry.getColumn(0);
//获取表头行对象
IRow headRow = kdtEntry.getHeadRow(0);
//获取表体行对象
IRow row = kdtEntry.getRow(0);
//获取单元对象
ICell cell = row.getCell(0);
```
#### 设置单元格的值
```java
//获取单元对象
cell.setValue(value);
```
#### 修改列、行、单元格样式
```java
//设置列隐藏
column.getStyleAttributes().setHided(true);
//设置行隐藏
row.getStyleAttributes().setHided(true);
//设置单元格背景颜色
cell.getStyleAttributes().setBackground(color);
//锁定行
column.getStyleAttributes().setLocked(true);
//设置单元格对其方式
cell.getStyleAttributes().setHorizontalAlign(HorizontalAlignment.RIGHT);
```
#### 修改行高、列宽
```java
//设置行高
kdtEntry.getRow(0).setHeight(100);
//设置列宽
kdtEntry.getColumn(0).setWidth(100);
```
#### 行融合
```java
KDTMergeManager mergeManager = kdtEntry.getMergeManager();
//不管值是否相等，强制融合
mergeManager.mergeBlock(0, 0, 1, 1, KDTMergeManager.SPECIFY_MERGE);
```
#### 表格文本自动换行
```java
protected void appendFootRow(KDTable table) {
	super.appendFootRow(table);
	kdtEntry.getColumn(1).getStyleAttributes().setWrapText(true);//设置第一列为自动换行
	kdtEntry.getColumn(1).setWidth(440); //设置第一列宽度
	kdtEntry.setDefaultRowHeight(55);	//设置行高度
}
```
#### 设置分录合计行
```java
//覆盖方法
@Overriod
protected void setTableToSumField() {
    super.setTableToSumField();
    setTableToSumField(kdtEntry, new String[] {"qty", "amount", "tax", "taxAmount"});//数组中传入要统计的列
}
```
#### 设置分录F7
```java
KDBizPromptBox pmptBox = new KDBizPromptBox();
pmptBox = new KDBizPromptBox();
pmptBox.setQueryInfo("com.kingdee.eas.hr.rec.app.CompanyF7Query");
pmptBox.setEditFormat("$number$");
pmptBox.setCommitFormat("$number$");
pmptBox.setDisplayFormat("$name$");
kdtEntries.getColumn("company").setEditor(new KDTDefaultCellEditor(pmptBox));
```
#### 获取表格F7
//具体F7设置请参考对应章节
```java
KDBizPromptBox f7Factory = (KDBizPromptBox) tbl.getColumn("factory").getEditor().getComponent();
```
#### 获取表格选中行
//可参考com.kingdee.eas.util.client.KDTableUtil类
```java
public static int[] getSelectedRows(KDTable table){
	if (table.getSelectManager().size() == 0) {
		return new int[0];
	}

	int count = getSelectedRowCount(table);
	int[] rows = new int[count];
	int k = 0;
	for (int i = 0; i < table.getSelectManager().size(); ++i) {
		KDTSelectBlock block = table.getSelectManager().get(i);
		for (int j = block.getTop(); j <= block.getBottom(); ++j) {
			rows[k] = j;
			++k;
		}
	}
	return rows;
}
public static int getSelectedRowCount(KDTable table){
	int count = 0;
	for (int i = 0; i < table.getSelectManager().size(); ++i) {
		KDTSelectBlock block = table.getSelectManager().get(i);
		count += block.getBottom() - block.getTop() + 1;
	}
	return count;
}
```
#### 校验分录必录
//可参考com.kingdee.eas.st.common.util.UIHelper类
```java
public static void verifyTableRequire(CoreUIObject ui, String tableName,
		KDTable table, boolean isEntryNotNull) {
	if (ui == null || table == null) {
		return;
	}
	if (tableName == null) {
		tableName = EASResource.getString(resource, "Entries");
	}
	IColumn column = null;
	ICell cell = null;
	int rows = table.getRowCount();
	if (isEntryNotNull && rows <= 0) {
		// MsgBox.showWarning(tableName + "不能为空");
		MsgBox.showWarning(tableName
				+ EASResource.getString(resource, "IsNotNull"));
		SysUtil.abort();
	}
	int columns = table.getColumnCount();
	for (int i = 0; i < columns; i++) {
		column = table.getColumn(i);
		if (column != null && column.isRequired()) {
			for (int j = 0; j < rows; j++) {
				cell = table.getCell(j, i);
				if (cell == null || cell.getValue() == null) {
					MsgBox.showWarning(ui, tableName
							+ EASResource.getString(resource, "First")
							+ (j + 1)
							+ EASResource.getString(resource, "Line")
							+ table.getHeadRow(0).getCell(i).getValue()
							+ EASResource.getString(resource, "IsNotNull"));
					SysUtil.abort();
				}
			}
		}
	}
}
```
#### 表格数据格式
设置列格式的方法：table.getColumn(colIndex).getStyleAttributes().setNumberFormat(formatString);
目前KDTable已能支持Excel2003的格式串，只有个缺陷：格式串中有中文导出尚有问题，中文变乱码， 建议将来都使用Excel2003的格式串，但旧的格式化串还支持，但是如果该表需要导出到excel，必须使用新的格式串，否则导出到excel，可能会显示不一致。
文本类：
1、@ 指定内容按文本显示，主要用于编码、手机号等用数字表示的文本。设定该格式后，可以保证导出excel时，此类文本不会被转成数字显示。
数值类：
1、0.00 表示两位小数,例如3.10367显示为3.10
2、0.## 表示两位小数，当小数末位为0时，0将不显示。例如3.10显示为3.1
3、"#,##0.00 "表示两位小数，且显示千份位
4、#,##0.00;[Red]#,##0.00 表示负数红字
5、0.00;[Red]0.00;" " 表示负数红字，且数据为0时不显示
6、0.00;[Red](0.00);" "表示正数时两位小数，负数时两位小数并显示红色，0时不显示。0.00;[Red](0.00)只是一个示例，可以为任意的数字格式串，后边再加上;" "(空格)即表示数据为0时不显示。
日期类：
1、 yyyy-m-d
2、 yyyy-MM-dd
4、 yyyy年MM月dd日
百分比：
1、0%
2、0.00%
例子
```java
1、由数字组成的长字符串导出excel后显示为科学计数法或字符串显示不完整，例如手机号13433445678。 
解决办法：给KDTable的列设置格式串(col.getStyleAttributes().setNumberFormat("@"))，指定该列为字符型即可。 
2、数字位过多的大数字导出excel后显示为科学计数法或精度丢失。 
解决办法：给KDTable的列设置格式串(col.getStyleAttributes().setNumberFormat("0.00"))。
这里的0.00只是示例，数字格式还有很多种
3、日期类型数据导出excel后显示格式不正确。 
解决办法：给KDTable的列设置格式串(col.getStyleAttributes().setNumberFormat("yyyy-MM-dd"))。
```
#### 表格单元格复制时只复制值
```java
this.kdtEntry.getEditHelper().setCoypMode(KDTEditHelper.VALUE);
```


### 表格事件
- #### 表格点击事件
```java
this.kdtEntry.addKDTMouseListener(new KDTMouseListener() {
    public void tableClicked(KDTMouseEvent e) {
        try {
            kdtEntry_tableClicked(e);
        } catch (Exception exc) {
            handUIException(exc);
        } finally {
        }
    }
});
```
#### 表格编辑结束事件
```java
this.kdtEntry.addKDTEditListener(new KDTEditAdapter() {
    public void editStopped(KDTEditEvent e) {
        try {
            kdtEntry_editStopped(e);
        } catch(Exception exc) {
            handUIException(exc);
        }
    }
});
```
#### 表格分录按钮事件
```java
IDetailPanelListener Entry_detailPanelAddListener=null;
IDetailPanelListener Entry_detailPanelInsertListener=null;
IDetailPanelListener Entry_detailPanelRemoveListener=null;
protected void kdtEntrySetValue(){
	//添加新增事件
	if(Entry_detailPanelAddListener==null){
		Entry_detailPanelAddListener = new IDetailPanelListener(){
			public void afterEvent(DetailPanelEvent e) throws Exception {
	
			}
			public void beforeEvent(DetailPanelEvent e) throws Exception {
	     		//新增分录时赋默认值
				IObjectValue vo = e.getObjectValue();
				vo.put("taxRate", 17);
				vo.put("haveRecGoods", 0);
				vo.put("notRecGoods", 0);
				vo.put("rowState",purRowStatus.addNew);
			}
		};
	}
	 //添加插入事件
	if(Entry_detailPanelInsertListener==null){
		Entry_detailPanelInsertListener = new IDetailPanelListener(){
			public void afterEvent(DetailPanelEvent e) throws Exception {
	
			}
			public void beforeEvent(DetailPanelEvent e) throws Exception {
	
			}
		};
	}
	//添加删除事件
	if(Entry_detailPanelRemoveListener==null){
		Entry_detailPanelRemoveListener = new IDetailPanelListener(){
			public void afterEvent(DetailPanelEvent e) throws Exception {
	
			}
			public void beforeEvent(DetailPanelEvent e) throws Exception {
	
			}
		};
	}
	//添加监听器方法
	kdtEntry_detailPanel.addInsertListener(Entry_detailPanelInsertListener);
	kdtEntry_detailPanel.addAddListener(Entry_detailPanelAddListener);
	kdtEntry_detailPanel.addRemoveListener(Entry_detailPanelRemoveListener);
}
```
