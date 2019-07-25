---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 96e96380438c290825861d1c1a5fd1fc9ab17236
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35707797"
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