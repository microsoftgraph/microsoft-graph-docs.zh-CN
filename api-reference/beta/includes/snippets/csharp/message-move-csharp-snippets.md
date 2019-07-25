---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3746628347e22d4c4bb86cf57367dc04b212bb59
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721425"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var destinationId = "deleteditems";

await graphClient.Me.Messages["AAMkADhAAATs28OAAA="]
    .Move(destinationId)
    .Request()
    .PostAsync();

```