---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7397d4ee37137ecb1f54270f18e91198e42d10c1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796549"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "Cancelling for this week due to all hands";

await graphClient.Me.Events["{event-id}"]
    .Cancel(comment)
    .Request()
    .PostAsync();

```