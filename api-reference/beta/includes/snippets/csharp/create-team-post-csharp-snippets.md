---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 444199ebba343e829706edf90b5de2b6aa4446ba
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335433"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var team = new Team
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"template@odata.bind","https://graph.microsoft.com/beta/teamsTemplates('standard')"}
    },
    DisplayName = "My Sample Team",
    Description = "My Sample Team’s Description"
};

await graphClient.Teams
    .Request()
    .AddAsync(team);

```