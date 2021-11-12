---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64460095e1c9c50e89a477cff5fc5305dd1964aeb2896f008bf1746ede73ea48
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278138"
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