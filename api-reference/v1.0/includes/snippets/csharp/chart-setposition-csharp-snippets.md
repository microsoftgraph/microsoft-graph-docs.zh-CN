---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 53a419e0f7c44e0b048eeaef0ca499b537b9e938
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53581099"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var startCell = JsonDocument.Parse(@"""startCell-value""");

var endCell = JsonDocument.Parse(@"""endCell-value""");

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"]
    .SetPosition(startCell,endCell)
    .Request()
    .PostAsync();

```