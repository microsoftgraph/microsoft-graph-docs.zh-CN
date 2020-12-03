---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16abd6244b4b7dfe29b484a56ba4ce1ef3e307f1
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522919"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationMember = new AadUserConversationMember
{
    Roles = new List<String>()
    {
        "owner"
    },
    AdditionalData = new Dictionary<string, object>()
    {
        {"user@odata.bind", "https://graph.microsoft.com/v1.0/users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')"}
    }
};

await graphClient.Teams["ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062"].Members
    .Request()
    .AddAsync(conversationMember);

```