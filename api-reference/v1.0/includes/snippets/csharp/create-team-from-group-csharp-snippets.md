---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 743d9775392f03bccf19e3bc9252a38319e5b501
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48374047"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var team = new Team
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"template@odata.bind", "https://graph.microsoft.com/v1.0/teamsTemplates('standard')"},
        {"group@odata.bind", "https://graph.microsoft.com/v1.0/groups('groupId')"}
    }
};

await graphClient.Teams
    .Request()
    .AddAsync(team);

```