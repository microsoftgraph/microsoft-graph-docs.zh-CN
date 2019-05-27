---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cff39086239a50316ffc02af62b1d0c356e7f1ad
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34462418"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookNamedItem = new WorkbookNamedItem
{
    Type = "type-value",
    Scope = "scope-value",
    Comment = "comment-value",
    Value = new Json
    {
    },
    Visible = true
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Request()
    .UpdateAsync(workbookNamedItem);

```