---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd40d2d91f6d481a30dd2728fd3c5966d571171d
ms.sourcegitcommit: 997fbfe36b518e0a8c230ae2e62666bb5c829e7e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/19/2019
ms.locfileid: "37045340"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "comment-value";

var sendResponse = true;

await graphClient.Me.Events["{id}"]
    .Accept(sendResponse,comment)
    .Request()
    .PostAsync();

```