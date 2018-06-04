# <a name="display-a-chart-image-in-excel-with-microsoft-graph"></a>通过 Microsoft Graph 显示 Excel 图表图像

在执行 [GET 操作以检索图表图像](/api-reference/v1.0/api/chart_image.md)时，Excel API 将返回 base-64 字符串形式的图像。

可以在 HTML 图像标记内显示 base-64 字符串：`<img src="data:image/png;base64,{base-64 chart image string}/>`。

对于默认行为，请使用 `Image(width=0,height=0,fittingMode='fit')`。 下面的示例展示了使用默认参数返回的图表图像。

![使用默认高度和宽度的 Excel 图表图像。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

若要自定义图像的显示方式，请指定高度、宽度和调整模式。 下面展示了使用 `Image(width=500,height=500,fittingMode='Fill')` 参数检索的同一个图表图像。

## <a name="see-also"></a>另请参阅

* [通过 Microsoft Graph 管理 Excel 会话](excel-manage-sessions.md)
* [使用 Microsoft Graph 编写 Excel 工作簿](excel-write-to-workbook.md)
* [通过 Microsoft Graph 使用 Excel 工作簿函数](excel-use-functions.md)
* [通过 Microsoft Graph 更新 Excel 区域的格式](excel-update-range-format.md)
* [使用 Excel REST API](../api-reference/v1.0/resources/excel.md)
