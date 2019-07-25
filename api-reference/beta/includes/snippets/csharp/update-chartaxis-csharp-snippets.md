---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0e60d1d547ea8bbf50615c0cf7b907d3142e14a7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708348"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartAxis = new WorkbookChartAxis
{
    MajorUnit = new Json
    {
    },
    Maximum = new Json
    {
    },
    Minimum = new Json
    {
    }
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Axes.ValueAxis
    .Request()
    .UpdateAsync(workbookChartAxis);

```