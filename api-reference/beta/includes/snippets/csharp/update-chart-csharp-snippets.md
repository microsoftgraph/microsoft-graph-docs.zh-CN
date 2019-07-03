---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 749ecae73c2aeba28b2234705fa4a153b034721c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479359"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChart = new WorkbookChart
{
    Height = 99,
    Left = 99
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"]
    .Request()
    .UpdateAsync(workbookChart);

```