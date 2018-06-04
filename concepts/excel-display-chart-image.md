# <a name="display-a-chart-image-in-excel-with-microsoft-graph"></a><span data-ttu-id="3da99-101">通过 Microsoft Graph 显示 Excel 图表图像</span><span class="sxs-lookup"><span data-stu-id="3da99-101">Display a chart image in Excel with Microsoft Graph</span></span>

<span data-ttu-id="3da99-102">在执行 [GET 操作以检索图表图像](/api-reference/v1.0/api/chart_image.md)时，Excel API 将返回 base-64 字符串形式的图像。</span><span class="sxs-lookup"><span data-stu-id="3da99-102">When you perform a [GET operation to retrieve a chart image](/api-reference/v1.0/api/chart_image.md), the Excel API returns the image as a base-64 string.</span></span>

<span data-ttu-id="3da99-103">可以在 HTML 图像标记内显示 base-64 字符串：`<img src="data:image/png;base64,{base-64 chart image string}/>`。</span><span class="sxs-lookup"><span data-stu-id="3da99-103">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="3da99-104">对于默认行为，请使用 `Image(width=0,height=0,fittingMode='fit')`。</span><span class="sxs-lookup"><span data-stu-id="3da99-104">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="3da99-105">下面的示例展示了使用默认参数返回的图表图像。</span><span class="sxs-lookup"><span data-stu-id="3da99-105">Here is an example of a chart image returned with the default parameters.</span></span>

![使用默认高度和宽度的 Excel 图表图像。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="3da99-107">若要自定义图像的显示方式，请指定高度、宽度和调整模式。</span><span class="sxs-lookup"><span data-stu-id="3da99-107">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="3da99-108">下面展示了使用 `Image(width=500,height=500,fittingMode='Fill')` 参数检索的同一个图表图像。</span><span class="sxs-lookup"><span data-stu-id="3da99-108">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

## <a name="see-also"></a><span data-ttu-id="3da99-109">另请参阅</span><span class="sxs-lookup"><span data-stu-id="3da99-109">See also</span></span>

* [<span data-ttu-id="3da99-110">通过 Microsoft Graph 管理 Excel 会话</span><span class="sxs-lookup"><span data-stu-id="3da99-110">Manage sessions in Excel with Microsoft Graph</span></span>](excel-manage-sessions.md)
* [<span data-ttu-id="3da99-111">使用 Microsoft Graph 编写 Excel 工作簿</span><span class="sxs-lookup"><span data-stu-id="3da99-111">Write to an Excel workbook using Microsoft Graph</span></span>](excel-write-to-workbook.md)
* [<span data-ttu-id="3da99-112">通过 Microsoft Graph 使用 Excel 工作簿函数</span><span class="sxs-lookup"><span data-stu-id="3da99-112">Use workbook functions in Excel with Microsoft Graph</span></span>](excel-use-functions.md)
* [<span data-ttu-id="3da99-113">通过 Microsoft Graph 更新 Excel 区域的格式</span><span class="sxs-lookup"><span data-stu-id="3da99-113">Update a range’s format in Excel with Microsoft Graph</span></span>](excel-update-range-format.md)
* [<span data-ttu-id="3da99-114">使用 Excel REST API</span><span class="sxs-lookup"><span data-stu-id="3da99-114">Use the Excel REST API</span></span>](../api-reference/v1.0/resources/excel.md)
