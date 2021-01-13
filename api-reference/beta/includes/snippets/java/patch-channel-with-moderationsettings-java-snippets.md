---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 45335cd82aa2e1e7e6900de4984b7e0a52770ff6
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49843678"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Channel channel = new Channel();
channel.displayName = "UpdateChannelModeration";
channel.description = "Update channel moderation.";
ChannelModerationSettings moderationSettings = new ChannelModerationSettings();
moderationSettings.userNewMessageRestriction = UserNewMessageRestriction.MODERATORS;
moderationSettings.replyRestriction = ReplyRestriction.EVERYONE;
moderationSettings.allowNewMessageFromBots = true;
moderationSettings.allowNewMessageFromConnectors = true;
channel.moderationSettings = moderationSettings;

graphClient.teams("{team-id}").channels("{channel-id}")
    .buildRequest()
    .patch(channel);

```