---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7420d86c860e0e521e0045556f2901e536f8544d
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681942"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var team = new Team
{
    DisplayName = "My Class Team",
    Description = "My Class Team’s Description",
    AdditionalData = new Dictionary<string, object>()
    {
        {"template@odata.bind", "https://graph.microsoft.com/beta/teamsTemplates('educationClass')"}
    }
};

await graphClient.Teams
    .Request()
    .AddAsync(team);

```