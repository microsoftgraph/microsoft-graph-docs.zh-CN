---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a9fdfde4fe4eb5230cc19d7375fc2ec914c5d38a316eae496e8b104001a69ba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904210"
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
    },
    DiscoverySettings = new TeamDiscoverySettings
    {
        ShowInTeamsSearchAndSuggestions = true
    }
};

await graphClient.Groups["{group-id}"].Team
    .Request()
    .PutAsync(team);

```