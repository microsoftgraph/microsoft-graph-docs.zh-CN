---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43002aa5108c27245d54a9a0086c2c3af7f60f8b
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509261"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var team = new Team
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"template@odata.bind", "https://graph.microsoft.com/v1.0/teamsTemplates('standard')"},
        {"group@odata.bind", "https://graph.microsoft.com/v1.0/groups('71392b2f-1765-406e-86af-5907d9bdb2ab')"}
    }
};

await graphClient.Teams
    .Request()
    .AddAsync(team);

```