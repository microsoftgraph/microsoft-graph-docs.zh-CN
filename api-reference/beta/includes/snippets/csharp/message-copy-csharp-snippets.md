---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 029c0ec73474c3a8fb2610b904187f66f40eaa3d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807172"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var destinationId = "destinationId-value";

await graphClient.Me.Messages["{message-id}"]
    .Copy(destinationId)
    .Request()
    .PostAsync();

```