---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4eb79a1631d036b91606869e6fd3b642bd68c6f6
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206867"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationMember = new AadUserConversationMember
{
    Roles = new List<String>()
    {
    },
    TenantId = "a18103d1-a6ef-4f66-ac64-e4ef42ea8681",
    AdditionalData = new Dictionary<string, object>()
    {
        {"user@odata.bind", "https://graph.microsoft.com/beta/users/bc3598dd-cce4-4742-ae15-173429951408"}
    }
};

await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Members
    .Request()
    .AddAsync(conversationMember);

```