---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72930e3cdbf504bc9391d7d0632e3afc4f99d9fe7b5dcce994efc66ac4a59514
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279693"
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
                {"user@odata.bind", "https://graph.microsoft.com/v1.0/users('62855810-484b-4823-9e01-60667f8b12ae')"}
            }
        }
    }
};

await graphClient.Teams["{team-id}"].Channels
    .Request()
    .AddAsync(channel);

```