---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c64ee9a03744e561d06d4395688df9f112d36512edd467b6d4bd41754a521ea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378601"
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