---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 705362dae2aeb010375664edb818144fbbb6a375
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46813680"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var team = new Team
{
    IsMembershipLimitedToOwners = true,
    MemberSettings = new TeamMemberSettings
    {
        AllowCreateUpdateChannels = true
    },
    MessagingSettings = new TeamMessagingSettings
    {
        AllowUserEditMessages = true,
        AllowUserDeleteMessages = true
    },
    FunSettings = new TeamFunSettings
    {
        AllowGiphy = true,
        GiphyContentRating = GiphyRatingType.Strict
    },
    DiscoverySettings = new TeamDiscoverySettings
    {
        ShowInTeamsSearchAndSuggestions = true
    }
};

await graphClient.Teams["{id}"]
    .Request()
    .UpdateAsync(team);

```