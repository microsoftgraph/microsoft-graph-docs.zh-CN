---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7604e371eaf0924732a1d20f6648d28a110b691e
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49692796"
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

await graphClient.Users["5b649834-7412-4cce-9e69-176e95a394f5"].Teamwork.InstalledApps
    .Request()
    .AddAsync(userScopeTeamsAppInstallation);

```