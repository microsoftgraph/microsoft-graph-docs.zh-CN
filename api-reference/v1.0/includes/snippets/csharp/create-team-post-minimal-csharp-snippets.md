---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57ae93fee5bf94d9dd8f23c93588533ff802e2fd
ms.sourcegitcommit: c4366ac71cf496242c8ff435bc8d8b3816bdc1aa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2020
ms.locfileid: "48315280"
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
        {"owners@odata.bind", "[\"https://graph.microsoft.com/v1.0/users('userId')\"]"}
    }
};

await graphClient.Teams
    .Request()
    .AddAsync(team);

```