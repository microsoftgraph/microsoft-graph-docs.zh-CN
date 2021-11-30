---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f34465cb6695b3b7cb8826843fecac4499f9ee64
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61225818"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = new TeamworkUserIdentity
{
    Id = "d864e79f-a516-4d0f-9fee-0eeb4d61fdc2"
};

var tenantId = "2a690434-97d9-4eed-83a6-f5f13600199a";

await graphClient.Chats["{chat-id}"]
    .UnhideForUser(user,tenantId)
    .Request()
    .PostAsync();

```