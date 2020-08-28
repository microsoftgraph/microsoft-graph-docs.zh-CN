---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cfac02afde353dd5e463551ec7c6b8314e1bc8e6
ms.sourcegitcommit: c4366ac71cf496242c8ff435bc8d8b3816bdc1aa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2020
ms.locfileid: "47287641"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var team = new Team
{
    DisplayName = "My Sample Team",
    Description = "My Sample Team’s Description",
    AdditionalData = new Dictionary<string, object>()
    {
        {"template@odata.bind", "https://graph.microsoft.com/beta/teamsTemplates('standard')"},
        {"members@odata.bind", "[{\"@odata.type\":\"#microsoft.graph.aadUserConversationMember\",\"roles\":[\"owner\"],\"userId\":\"0040b377-61d8-43db-94f5-81374122dc7e\"}]"}
    }
};

await graphClient.Teams
    .Request()
    .AddAsync(team);

```