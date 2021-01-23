---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7660f494f24187d408cf969ee78edb77646130f8
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945987"
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
                {"user@odata.bind", "https://graph.microsoft.com/beta/users('62855810-484b-4823-9e01-60667f8b12ae')"}
            }
        }
    }
};

await graphClient.Teams["57fb72d0-d811-46f4-8947-305e6072eaa5"].Channels
    .Request()
    .AddAsync(channel);

```