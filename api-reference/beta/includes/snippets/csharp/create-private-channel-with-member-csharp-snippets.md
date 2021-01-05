---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 45da67703848dca5528243eec761114a535ea133
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753816"
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
                {"user@odata.bind", "https://graph.microsoft.com/beta/users('62855810-484b-4823-9e01-60667f8b12ae')"}
            }
        }
    }
};

await graphClient.Teams["57fb72d0-d811-46f4-8947-305e6072eaa5"].Channels
    .Request()
    .AddAsync(channel);

```