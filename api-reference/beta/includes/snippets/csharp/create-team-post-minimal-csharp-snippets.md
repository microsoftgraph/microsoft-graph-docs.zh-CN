---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ed0950f9613d1a4376e7417273af2baf65842f7
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681959"
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
        {"owners@odata.bind", "[\"https://graph.microsoft.com/beta/users('userId')\"]"}
    }
};

await graphClient.Teams
    .Request()
    .AddAsync(team);

```