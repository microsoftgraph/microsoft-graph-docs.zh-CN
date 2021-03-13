---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a4e43c6375088de11ae9abaad6a4eb21bd0f1b1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786441"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "comment-value";

var sendResponse = true;

await graphClient.Me.Events["{event-id}"]
    .Accept(comment,sendResponse)
    .Request()
    .PostAsync();

```