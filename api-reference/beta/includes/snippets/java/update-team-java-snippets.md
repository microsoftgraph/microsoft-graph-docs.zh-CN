---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46f889bcabf837c136b61b7c97d12f14a5212061
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969036"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Team team = new Team();
team.isMembershipLimitedToOwners = true;
TeamMemberSettings memberSettings = new TeamMemberSettings();
memberSettings.allowCreateUpdateChannels = true;
team.memberSettings = memberSettings;
TeamMessagingSettings messagingSettings = new TeamMessagingSettings();
messagingSettings.allowUserEditMessages = true;
messagingSettings.allowUserDeleteMessages = true;
team.messagingSettings = messagingSettings;
TeamFunSettings funSettings = new TeamFunSettings();
funSettings.allowGiphy = true;
funSettings.giphyContentRating = GiphyRatingType.STRICT;
team.funSettings = funSettings;
TeamDiscoverySettings discoverySettings = new TeamDiscoverySettings();
discoverySettings.showInTeamsSearchAndSuggestions = true;
team.discoverySettings = discoverySettings;

graphClient.teams("{id}")
    .buildRequest()
    .patch(team);

```