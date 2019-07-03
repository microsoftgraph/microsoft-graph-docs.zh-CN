---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fd53ee903cb8e3802c1d752ebe9a41300d2cefd9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35480132"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartPoint = new WorkbookChartPoint
{
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Series["{undefined}"].Points
    .Request()
    .AddAsync(workbookChartPoint);

```