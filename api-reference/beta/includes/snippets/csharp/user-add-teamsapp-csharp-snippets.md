---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ad33e3529e5b28e704ffb0512c3202bf8625c8b
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684558"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsAppInstallation = new TeamsAppInstallation
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"teamsApp@odata.bind", "https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"}
    }
};

await graphClient.Users["{id}"].Teamwork.InstalledApps
    .Request()
    .AddAsync(teamsAppInstallation);

```