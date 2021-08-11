---
title: 通过 Microsoft Graph 显示 Excel 图表图像
description: 如果你通过执行 GET 操作来检索图表图像，Excel API 便会以 base-64 字符串形式返回图像。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 6e456a8008eb3d50da818c2e3da1a48ca54f4211eb5b1e8300dd3bef6dbf5e59
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54149567"
---
# <a name="display-a-chart-image-in-excel-with-microsoft-graph"></a>通过 Microsoft Graph 在 Excel 中显示图表图像

在执行 [GET 操作以检索图表图像](/graph/api/chart-image?view=graph-rest-1.0)时，Excel API 将返回 base-64 字符串形式的图像。

可以在 HTML 图像标记内显示 base-64 字符串：`<img src="data:image/png;base64,{base-64 chart image string}/>`。

对于默认行为，请使用 `Image(width=0,height=0,fittingMode='fit')`。 下面的示例展示了使用默认参数返回的图表图像。

![使用默认高度和宽度的 Excel 图表图像。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

若要自定义图像的显示方式，请指定高度、宽度和调整模式。 下面展示了使用 `Image(width=500,height=500,fittingMode='Fill')` 参数检索的同一个图表图像。

## <a name="see-also"></a>另请参阅

* [通过 Microsoft Graph 管理 Excel 会话](excel-manage-sessions.md)
* [使用 Microsoft Graph 编写 Excel 工作簿](excel-write-to-workbook.md)
* [通过 Microsoft Graph 使用 Excel 工作簿函数](excel-use-functions.md)
* [通过 Microsoft Graph 更新 Excel 区域的格式](excel-update-range-format.md)
* [使用 Excel REST API](/graph/api/resources/excel?view=graph-rest-1.0)
