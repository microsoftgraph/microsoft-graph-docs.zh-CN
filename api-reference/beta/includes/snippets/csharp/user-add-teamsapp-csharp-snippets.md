---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb4a721a605a0337a35733fe47e0644ab364eca6
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46569976"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userScopeTeamsAppInstallation = new UserScopeTeamsAppInstallation
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"teamsApp@odata.bind", "https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"}
    }
};

await graphClient.Users["{id}"].Teamwork.InstalledApps
    .Request()
    .AddAsync(userScopeTeamsAppInstallation);

```