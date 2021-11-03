---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d8c80f6e5144117262cb6be7483a8b74634afb5
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695731"
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
                {"user@odata.bind", "https://graph.microsoft.com/v1.0/users('jacob@contoso.com')"}
            }
        }
    },
    AdditionalData = new Dictionary<string, object>()
    {
        {"template@odata.bind", "https://graph.microsoft.com/v1.0/teamsTemplates('standard')"}
    }
};

await graphClient.Teams
    .Request()
    .AddAsync(team);

```