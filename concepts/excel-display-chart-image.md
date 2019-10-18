---
title: 通过 Microsoft Graph 显示 Excel 图表图像
description: 如果你通过执行 GET 操作来检索图表图像，Excel API 便会以 base-64 字符串形式返回图像。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 330c7d3a531a5735e824dda61928c3af2f05e5e3
ms.sourcegitcommit: ca55fc5f5711966eaa41da31cd1ae99820e9e586
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2019
ms.locfileid: "35645211"
---
# <a name="display-a-chart-image-in-excel-with-microsoft-graph"></a><span data-ttu-id="c6f71-103">通过 Microsoft Graph 在 Excel 中显示图表图像</span><span class="sxs-lookup"><span data-stu-id="c6f71-103">Display a chart image in Excel with Microsoft Graph</span></span>

<span data-ttu-id="c6f71-104">在执行 [GET 操作以检索图表图像](/graph/api/chart-image?view=graph-rest-1.0)时，Excel API 将返回 base-64 字符串形式的图像。</span><span class="sxs-lookup"><span data-stu-id="c6f71-104">When you perform a [GET operation to retrieve a chart image](/graph/api/chart-image?view=graph-rest-1.0), the Excel API returns the image as a base-64 string.</span></span>

<span data-ttu-id="c6f71-105">可以在 HTML 图像标记内显示 base-64 字符串：`<img src="data:image/png;base64,{base-64 chart image string}/>`。</span><span class="sxs-lookup"><span data-stu-id="c6f71-105">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="c6f71-106">对于默认行为，请使用 `Image(width=0,height=0,fittingMode='fit')`。</span><span class="sxs-lookup"><span data-stu-id="c6f71-106">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="c6f71-107">下面的示例展示了使用默认参数返回的图表图像。</span><span class="sxs-lookup"><span data-stu-id="c6f71-107">Here is an example of a chart image returned with the default parameters.</span></span>

![使用默认高度和宽度的 Excel 图表图像。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="c6f71-109">若要自定义图像的显示方式，请指定高度、宽度和调整模式。</span><span class="sxs-lookup"><span data-stu-id="c6f71-109">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="c6f71-110">下面展示了使用 `Image(width=500,height=500,fittingMode='Fill')` 参数检索的同一个图表图像。</span><span class="sxs-lookup"><span data-stu-id="c6f71-110">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

## <a name="see-also"></a><span data-ttu-id="c6f71-111">另请参阅</span><span class="sxs-lookup"><span data-stu-id="c6f71-111">See also</span></span>

* [<span data-ttu-id="c6f71-112">通过 Microsoft Graph 管理 Excel 会话</span><span class="sxs-lookup"><span data-stu-id="c6f71-112">Manage sessions in Excel with Microsoft Graph</span></span>](excel-manage-sessions.md)
* [<span data-ttu-id="c6f71-113">使用 Microsoft Graph 编写 Excel 工作簿</span><span class="sxs-lookup"><span data-stu-id="c6f71-113">Write to an Excel workbook using Microsoft Graph</span></span>](excel-write-to-workbook.md)
* [<span data-ttu-id="c6f71-114">通过 Microsoft Graph 使用 Excel 工作簿函数</span><span class="sxs-lookup"><span data-stu-id="c6f71-114">Use workbook functions in Excel with Microsoft Graph</span></span>](excel-use-functions.md)
* [<span data-ttu-id="c6f71-115">通过 Microsoft Graph 更新 Excel 区域的格式</span><span class="sxs-lookup"><span data-stu-id="c6f71-115">Update a range’s format in Excel with Microsoft Graph</span></span>](excel-update-range-format.md)
* [<span data-ttu-id="c6f71-116">使用 Excel REST API</span><span class="sxs-lookup"><span data-stu-id="c6f71-116">Use the Excel REST API</span></span>](/graph/api/resources/excel?view=graph-rest-1.0)
