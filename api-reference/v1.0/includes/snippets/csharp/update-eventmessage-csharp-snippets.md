---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16d57fed848c6fa76e1c5eeb8459071e0446fe2f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787670"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    IsRead = true
};

await graphClient.Me.Messages["{message-id}"]
    .Request()
    .UpdateAsync(message);

```