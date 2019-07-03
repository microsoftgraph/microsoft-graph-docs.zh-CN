---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5a4787b9c0e0e3c395f55e1d980174f20e18ffef
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463533"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartGridlines = new WorkbookChartGridlines
{
    Visible = true
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Axes.ValueAxis.MinorGridlines
    .Request()
    .UpdateAsync(workbookChartGridlines);

```