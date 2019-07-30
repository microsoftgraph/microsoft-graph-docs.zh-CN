---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1c90634f69a349e4d442a827de2da72dcc3c8a0d
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931686"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsAppInstallation = new TeamsAppInstallation
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"teamsApp@odata.bind","https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"}
    }
};

await graphClient.Teams["87654321-0abc-zqf0-321456789q"].InstalledApps
    .Request()
    .AddAsync(teamsAppInstallation);

```