---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ad57b5398c9f726343c9504abdefcce3dd8e899
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806419"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userScopeTeamsAppInstallation = new UserScopeTeamsAppInstallation
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"teamsApp@odata.bind", "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"}
    }
};

await graphClient.Users["{user-id}"].Teamwork.InstalledApps
    .Request()
    .AddAsync(userScopeTeamsAppInstallation);

```