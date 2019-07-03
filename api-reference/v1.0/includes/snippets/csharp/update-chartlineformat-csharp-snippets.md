---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 78a2ad327cba2d6aec1a335e27d52605dade3b74
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493658"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartLineFormat = new WorkbookChartLineFormat
{
    Color = "color-value"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Axes.SeriesAxis.Format.Line
    .Request()
    .UpdateAsync(workbookChartLineFormat);

```