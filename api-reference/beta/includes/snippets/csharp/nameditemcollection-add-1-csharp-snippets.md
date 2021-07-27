---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c310d24c8c01b1f3349bda51498582741cd0280
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53581309"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var name = "test5";

var reference = JsonDocument.Parse(@"""=Sheet1!$F$15:$N$27""");

var comment = "Comment for the named item";

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names
    .Add(name,reference,comment)
    .Request()
    .PostAsync();

```