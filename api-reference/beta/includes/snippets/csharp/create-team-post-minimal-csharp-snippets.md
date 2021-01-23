---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ee55d8b2c5f6c684ec4000adeb079f07c6189f0
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945160"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var team = new Team
{
    DisplayName = "My Sample Team",
    Description = "My Sample Team’s Description",
    Members = new TeamMembersCollectionPage()
    {
        new AadUserConversationMember
        {
            Roles = new List<String>()
            {
                "owner"
            },
            AdditionalData = new Dictionary<string, object>()
            {
                {"user@odata.bind", "https://graph.microsoft.com/beta/users('0040b377-61d8-43db-94f5-81374122dc7e')"}
            }
        }
    },
    AdditionalData = new Dictionary<string, object>()
    {
        {"template@odata.bind", "https://graph.microsoft.com/beta/teamsTemplates('standard')"}
    }
};

await graphClient.Teams
    .Request()
    .AddAsync(team);

```