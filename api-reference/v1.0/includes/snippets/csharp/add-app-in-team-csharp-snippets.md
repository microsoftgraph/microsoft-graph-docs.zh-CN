---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5003c3b52ffc10db09b99bce28a550fc05ba6cd5089c7e1c4edf45fe1a3db51
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161975"
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

await graphClient.Teams["{team-id}"].InstalledApps
    .Request()
    .AddAsync(teamsAppInstallation);

```