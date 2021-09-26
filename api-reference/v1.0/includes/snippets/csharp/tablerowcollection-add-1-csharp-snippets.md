---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be61bcb54ab8f58bf1aebe27bd7b02d97c56976d
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59763863"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookTableRow = new WorkbookTableRow
{
    Values = JsonDocument.Parse(@"""[\r\n    [1, 2, 3],\r\n    [4, 5, 6]\r\n  ]""")
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Rows
    .Request()
    .Header("Prefer","respond-async")
    .Header("Workbook-Session-Id","{Workbook-Session-Id}")
    .AddAsync(workbookTableRow);

```