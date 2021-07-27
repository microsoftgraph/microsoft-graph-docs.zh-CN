---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 183acdad9e4c653748c1e17fb40b8c8a08bde5b5
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53581390"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var index = 3;

var values = JsonDocument.Parse("[{}]");

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Columns
    .Add(index,values,null)
    .Request()
    .PostAsync();

```