---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e22caa17cc852afbdf8745577ac9cfd4c282297
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48621861"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartDataLabels = new WorkbookChartDataLabels
{
    Position = "position-value",
    ShowValue = true,
    ShowSeriesName = true,
    ShowCategoryName = true,
    ShowLegendKey = true
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].DataLabels
    .Request()
    .UpdateAsync(workbookChartDataLabels);

```