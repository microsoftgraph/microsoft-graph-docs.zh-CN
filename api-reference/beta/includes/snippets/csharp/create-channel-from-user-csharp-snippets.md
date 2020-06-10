---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ade23f661530ddd2ada8f8752218b3ddf48ac59
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684383"
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
                {"user@odata.bind", "https://graph.microsoft.com/beta/users('{user_id}')"}
            }
        }
    }
};

await graphClient.Teams["{group_id}"].Channels
    .Request()
    .AddAsync(channel);

```