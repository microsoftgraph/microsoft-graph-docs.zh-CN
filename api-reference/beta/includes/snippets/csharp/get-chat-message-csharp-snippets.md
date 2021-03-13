---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 10d0a8055618bf327e237430fc9917ddd45eacca
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789810"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessage = await graphClient.Me.Chats["{chat-id}"].Messages["{chatMessage-id}"]
    .Request()
    .GetAsync();

```