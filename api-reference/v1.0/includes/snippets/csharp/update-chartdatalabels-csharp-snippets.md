---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3e22caa17cc852afbdf8745577ac9cfd4c282297
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493227"
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