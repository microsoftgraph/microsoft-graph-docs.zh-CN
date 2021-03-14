---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b1d1d26940a24575362678812b73b6c619f4af1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787521"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "comment-value";

await graphClient.Me.Messages["{message-id}"]
    .ReplyAll(null,comment)
    .Request()
    .PostAsync();

```