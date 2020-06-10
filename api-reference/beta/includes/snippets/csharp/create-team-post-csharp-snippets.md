---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4838af8006757fb2142228c45120b6689f951880
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681953"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var team = new Team
{
    DisplayName = "My Sample Team",
    Description = "My Sample Team’s Description",
    AdditionalData = new Dictionary<string, object>()
    {
        {"template@odata.bind", "https://graph.microsoft.com/beta/teamsTemplates('standard')"}
    }
};

await graphClient.Teams
    .Request()
    .AddAsync(team);

```