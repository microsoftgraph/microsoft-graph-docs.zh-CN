---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3746628347e22d4c4bb86cf57367dc04b212bb59
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620936"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var destinationId = "deleteditems";

await graphClient.Me.Messages["AAMkADhAAATs28OAAA="]
    .Move(destinationId)
    .Request()
    .PostAsync();

```