---
title: 在 Excel 中显示图表图像
description: 检索图表图像时，Microsoft Graph 中的 Excel API 将图像返回为可在 HTML 映像标记中显示的 base-64 字符串。
ms.localizationpriority: medium
author: lumine2008
ms.prod: excel
ms.openlocfilehash: ac1713d017ee982c4df5fc89ff4a28dc4437a4cf
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440851"
---
# <a name="display-a-chart-image-in-excel"></a>在 Excel 中显示图表图像

执行 [GET 操作以检索图表图像](/graph/api/chart-image)时，Microsoft Graph 中的 Excel API 将图像返回为 base-64 字符串。 可以在 HTML 映像标记中显示 base-64 字符串：

```html
 <img src="data:image/png;base64,{base-64 chart image string}/>
```

对于默认行为，请使用 `Image(width=0,height=0,fittingMode='fit')`。

下面是使用默认参数返回的图表图像的示例。

![使用默认高度和宽度的 Excel 图表图像。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

若要自定义图像的显示方式，请指定高度、宽度和调整模式。 下面展示了使用 `Image(width=500,height=500,fittingMode='Fill')` 参数检索的同一个图表图像。

## <a name="see-also"></a>另请参阅

* [通过 Microsoft Graph 管理 Excel 会话](excel-manage-sessions.md)
* [使用 Microsoft Graph 编写 Excel 工作簿](excel-write-to-workbook.md)
* [通过 Microsoft Graph 使用 Excel 工作簿函数](excel-use-functions.md)
* [通过 Microsoft Graph 更新 Excel 区域的格式](excel-update-range-format.md)
* [使用 Excel REST API](/graph/api/resources/excel)
