---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 827c43302bff85a0d75e538199a8fd77a08f44b0
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37544175"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channel = new Channel
{
    MembershipType = ChannelMembershipType.Private,
    DisplayName = "My First Private Channel",
    Description = "This is my first private channels",
    Members = new List<ConversationMember>()
    {
        new AadUserConversationMember
        {
            AdditionalData = new Dictionary<string, object>()
            {
                {"user@odata.bind","https://graph.microsoft.com/beta/users('{user_id}')"}
            },
            Roles = new List<String>()
            {
                "owner"
            }
        }
    }
};

await graphClient.Teams["{group_id}"].Channels
    .Request()
    .AddAsync(channel);

```