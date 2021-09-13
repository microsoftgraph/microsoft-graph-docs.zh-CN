---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 60b44ad4aee3123d4bcb58681111a29c4041cbb2414b2807975dda3b87add99b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161965"
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