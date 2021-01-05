---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d119001589eb473a49a16dae4a853a6f621803a
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756110"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessage = new ChatMessage
{
    Body = new ItemBody
    {
        Content = "Hello world"
    }
};

await graphClient.Chats["{id}"].Messages
    .Request()
    .AddAsync(chatMessage);

```