---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9095d5e36873656dd66b4feb5f33dbadb64716b52e8ce732840008b31c42880f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103744"
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