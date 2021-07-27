---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cdaad5de4cb7b80a4096cda3b3597d083590efa3
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53581212"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sourceData = JsonDocument.Parse(@"""sourceData-value""");

var seriesBy = "seriesBy-value";

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"]
    .SetData(seriesBy,sourceData)
    .Request()
    .PostAsync();

```