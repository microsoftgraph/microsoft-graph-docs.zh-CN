---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82b02d138cdb3b975f6b621855af33875238d42731d13d869983a18efc9171b8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378600"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var team = new Team
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"template@odata.bind", "https://graph.microsoft.com/beta/teamsTemplates('standard')"},
        {"group@odata.bind", "https://graph.microsoft.com/beta/groups('71392b2f-1765-406e-86af-5907d9bdb2ab')"}
    }
};

await graphClient.Teams
    .Request()
    .AddAsync(team);

```