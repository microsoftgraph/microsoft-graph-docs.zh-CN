---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 03dc191cc6983f27785fd555a073b91d5eab97a6
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633908"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationMember = new ConversationMember
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"user@odata.bind","https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"},
        {"@odata.type","microsoft.graph.aadConversationMember"}
    },
    Roles = new List<String>()
    {
    }
};

await graphClient.Teams["{id}"].Channels["{id}"].Members
    .Request()
    .AddAsync(conversationMember);

```