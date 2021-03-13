---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ec8e9483341a061c3e36079804e856f2ef5544b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779780"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartAxis = new WorkbookChartAxis
{
    MajorUnit = JToken.Parse("{}"),
    Maximum = JToken.Parse("{}"),
    Minimum = JToken.Parse("{}")
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"].Axes.ValueAxis
    .Request()
    .UpdateAsync(workbookChartAxis);

```