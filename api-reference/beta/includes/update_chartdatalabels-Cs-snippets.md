---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3e22caa17cc852afbdf8745577ac9cfd4c282297
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34457015"
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