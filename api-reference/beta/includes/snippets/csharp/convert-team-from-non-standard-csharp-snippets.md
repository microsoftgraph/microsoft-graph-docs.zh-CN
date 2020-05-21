---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b530dbb53ac9158eede15a1e3b5ada20e91590ea
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335448"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var team = new Team
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"template@odata.bind","https://graph.microsoft.com/beta/teamsTemplates('educationClass')"}
    },
    DisplayName = "My Class Team",
    Description = "My Class Team’s Description"
};

await graphClient.Teams
    .Request()
    .AddAsync(team);

```