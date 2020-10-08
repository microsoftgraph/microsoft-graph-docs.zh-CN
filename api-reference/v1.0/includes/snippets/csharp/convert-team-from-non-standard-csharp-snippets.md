---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 503a66f948b918f83feefa3e2533dc966477569a
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48374046"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var team = new Team
{
    DisplayName = "My Class Team",
    Description = "My Class Team’s Description",
    AdditionalData = new Dictionary<string, object>()
    {
        {"template@odata.bind", "https://graph.microsoft.com/v1.0/teamsTemplates('educationClass')"}
    }
};

await graphClient.Teams
    .Request()
    .AddAsync(team);

```