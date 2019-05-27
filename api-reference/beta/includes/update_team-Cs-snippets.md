---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3488a2dd545cb9ec6f8e80604b9830779c3e6388
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34475876"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var team = new Team
{
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
    }
};

await graphClient.Teams["{id}"]
    .Request()
    .UpdateAsync(team);

```