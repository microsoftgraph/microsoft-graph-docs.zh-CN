---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7da596600fee5f1c1eb7a4caf215f4e1022ac5fa
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753788"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channel = new Channel
{
    DisplayName = "TestChannelModeration",
    Description = "Test channel moderation.",
    MembershipType = ChannelMembershipType.Standard,
    ModerationSettings = new ChannelModerationSettings
    {
        UserNewMessageRestriction = UserNewMessageRestriction.EveryoneExceptGuests,
        ReplyRestriction = ReplyRestriction.Everyone,
        AllowNewMessageFromBots = true,
        AllowNewMessageFromConnectors = true
    }
};

await graphClient.Teams["57fb72d0-d811-46f4-8947-305e6072eaa5"].Channels
    .Request()
    .AddAsync(channel);

```