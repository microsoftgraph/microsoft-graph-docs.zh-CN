---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7c83111893a9bc7adefd6513e948b8d35bda08c
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373452"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channel = new Channel
{
    MembershipType = ChannelMembershipType.Private,
    DisplayName = "My First Private Channel",
    Description = "This is my first private channels",
    Members = (IChannelMembersCollectionPage)new List<ConversationMember>()
    {
        new AadUserConversationMember
        {
            Roles = new List<String>()
            {
                "owner"
            },
            AdditionalData = new Dictionary<string, object>()
            {
                {"user@odata.bind", "https://graph.microsoft.com/v1.0/users('{user_id}')"}
            }
        }
    }
};

await graphClient.Teams["{group_id}"].Channels
    .Request()
    .AddAsync(channel);

```