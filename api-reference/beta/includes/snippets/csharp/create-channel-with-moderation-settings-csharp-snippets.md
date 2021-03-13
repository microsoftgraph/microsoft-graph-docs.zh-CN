---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1fdb1fe15265ca98337582d75789d2c9e89fddeb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794685"
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

await graphClient.Teams["{team-id}"].Channels
    .Request()
    .AddAsync(channel);

```