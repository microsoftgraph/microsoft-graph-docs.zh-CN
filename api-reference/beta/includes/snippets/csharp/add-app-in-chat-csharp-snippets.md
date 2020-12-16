---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b44fc0c9d215473313a5228cd3dde5ac2755e21d
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689772"
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

await graphClient.Chats["19:ea28e88c00e94c7786b065394a61f296@thread.v2"].InstalledApps
    .Request()
    .AddAsync(teamsAppInstallation);

```