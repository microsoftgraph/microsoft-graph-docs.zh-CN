---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c5d7f85f81136c3671415735c9dc0cda49c6c0418e387b683ce9d8885942b65
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903222"
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