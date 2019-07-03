---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 96e96380438c290825861d1c1a5fd1fc9ab17236
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479602"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartTitle = new WorkbookChartTitle
{
    Overlay = true,
    Text = "text-value",
    Visible = true
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Title
    .Request()
    .UpdateAsync(workbookChartTitle);

```