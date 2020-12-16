---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc3e9f5d06206557f6227252df46787a8dc51ee5
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689626"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var values = new List<ConversationMember>()
{
    new AadUserConversationMember
    {
        Roles = new List<String>()
        {
        },
        AdditionalData = new Dictionary<string, object>()
        {
            {"user@odata.bind", "https://graph.microsoft.com/beta/users('18a80140-b0fb-4489-b360-2f6efaf225a0')"}
        }
    },
    new AadUserConversationMember
    {
        Roles = new List<String>()
        {
            "owner"
        },
        AdditionalData = new Dictionary<string, object>()
        {
            {"user@odata.bind", "https://graph.microsoft.com/beta/users('86503198-b81b-43fe-81ee-ad45b8848ac9')"}
        }
    }
};

await graphClient.Teams["e4183b04-c9a2-417c-bde4-70e3ee46a6dc"].Members
    .Add(values)
    .Request()
    .PostAsync();

```