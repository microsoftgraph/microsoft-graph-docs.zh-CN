---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 373e15eb48dcae40b03689900d1311cdd3f1a989
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684278"
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

await graphClient.Teams["87654321-0abc-zqf0-321456789q"].InstalledApps
    .Request()
    .AddAsync(teamsAppInstallation);

```