---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b69938e1cf66902a2cb4226d68e315595689b3f3
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53581369"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartAxis = new WorkbookChartAxis
{
    MajorUnit = JsonDocument.Parse("{}"),
    Maximum = JsonDocument.Parse("{}"),
    Minimum = JsonDocument.Parse("{}")
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"].Axes.ValueAxis
    .Request()
    .UpdateAsync(workbookChartAxis);

```