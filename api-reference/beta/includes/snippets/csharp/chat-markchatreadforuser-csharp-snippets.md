---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b9852ebc8f853c7d5c590fc43fcb0956f69a38c
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890645"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = new TeamworkUserIdentity
{
    Id = "d864e79f-a516-4d0f-9fee-0eeb4d61fdc2"
};

var tenantId = "2a690434-97d9-4eed-83a6-f5f13600199a";

await graphClient.Chats["{chat-id}"]
    .MarkChatReadForUser(user,tenantId)
    .Request()
    .PostAsync();

```