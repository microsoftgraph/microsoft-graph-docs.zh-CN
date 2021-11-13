---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e82423a034fd0032327ec6aed25eb03a61852416
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890611"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = new TeamworkUserIdentity
{
    Id = "d864e79f-a516-4d0f-9fee-0eeb4d61fdc2"
};

var tenantId = "2a690434-97d9-4eed-83a6-f5f13600199a";

var lastMessageReadDateTime = DateTimeOffset.Parse("2021-05-27T22:13:01.577Z");

await graphClient.Chats["{chat-id}"]
    .MarkChatUnreadForUser(user,tenantId,lastMessageReadDateTime)
    .Request()
    .PostAsync();

```