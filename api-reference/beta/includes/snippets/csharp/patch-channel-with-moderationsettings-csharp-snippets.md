---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35fa265c69b96481505c0283a0d14ddda8741a25
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49843674"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channel = new Channel
{
    DisplayName = "UpdateChannelModeration",
    Description = "Update channel moderation.",
    ModerationSettings = new ChannelModerationSettings
    {
        UserNewMessageRestriction = UserNewMessageRestriction.Moderators,
        ReplyRestriction = ReplyRestriction.Everyone,
        AllowNewMessageFromBots = true,
        AllowNewMessageFromConnectors = true
    }
};

await graphClient.Teams["{team-id}"].Channels["{channel-id}"]
    .Request()
    .UpdateAsync(channel);

```