---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e19f60b08cdd52937d2d93c167b84d124ded8261
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48374026"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var team = new Team
{
    DisplayName = "My Sample Team",
    Description = "My Sample Team’s Description",
    AdditionalData = new Dictionary<string, object>()
    {
        {"template@odata.bind", "https://graph.microsoft.com/v1.0/teamsTemplates('standard')"},
        {"members@odata.bind", "[{\"@odata.type\":\"#microsoft.graph.aadUserConversationMember\",\"roles\":[\"owner\"],\"userId\":\"0040b377-61d8-43db-94f5-81374122dc7e\"}]"}
    }
};

await graphClient.Teams
    .Request()
    .AddAsync(team);

```