---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3072bd2a6fce25695afd9ddb4bdd3be9dcd6e5d6
ms.sourcegitcommit: 997fbfe36b518e0a8c230ae2e62666bb5c829e7e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/19/2019
ms.locfileid: "37045339"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "comment-value";

var sendResponse = true;

await graphClient.Me.Events["{id}"]
    .Decline(sendResponse,comment)
    .Request()
    .PostAsync();

```