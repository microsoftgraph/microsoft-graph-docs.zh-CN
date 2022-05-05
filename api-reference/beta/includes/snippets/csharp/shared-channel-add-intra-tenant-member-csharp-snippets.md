---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8dc1e8ced3c3cd25c15f3d7909485c6405a66e45
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206868"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationMember = new AadUserConversationMember
{
    Roles = new List<String>()
    {
    },
    AdditionalData = new Dictionary<string, object>()
    {
        {"user@odata.bind", "https://graph.microsoft.com/beta/users/24b3819b-4e1d-4f3e-86bd-e42b54d0b2b4"}
    }
};

await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Members
    .Request()
    .AddAsync(conversationMember);

```