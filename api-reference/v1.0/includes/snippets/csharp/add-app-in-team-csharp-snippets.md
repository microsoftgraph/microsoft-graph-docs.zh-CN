---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4462f8b2f820422b16e8e2ca293528646d26d18c
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691015"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsAppInstallation = new TeamsAppInstallation
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"teamsApp@odata.bind", "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"}
    }
};

await graphClient.Teams["87654321-0abc-zqf0-321456789q"].InstalledApps
    .Request()
    .AddAsync(teamsAppInstallation);

```