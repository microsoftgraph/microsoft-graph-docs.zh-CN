---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc8bd0ac527c5aedf56ce7083c4d39e5ac2cdb35
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694409"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channel = new Channel
{
    MembershipType = ChannelMembershipType.Private,
    DisplayName = "My First Private Channel",
    Description = "This is my first private channels",
    Members = new ChannelMembersCollectionPage()
    {
        new AadUserConversationMember
        {
            Roles = new List<String>()
            {
                "owner"
            },
            AdditionalData = new Dictionary<string, object>()
            {
                {"user@odata.bind", "https://graph.microsoft.com/v1.0/users('jacob@contoso.com')"}
            }
        }
    }
};

await graphClient.Teams["{team-id}"].Channels
    .Request()
    .AddAsync(channel);

```