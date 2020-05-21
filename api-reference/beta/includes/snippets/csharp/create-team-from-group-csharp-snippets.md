---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba293cf32a423db1adffd6c1df4b1332c87ba208
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335432"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var team = new Team
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"group@odata.bind","https://graph.microsoft.com/v1.0/groups('groupId')"},
        {"template@odata.bind","https://graph.microsoft.com/beta/teamsTemplates('standard')"}
    }
};

await graphClient.Teams
    .Request()
    .AddAsync(team);

```