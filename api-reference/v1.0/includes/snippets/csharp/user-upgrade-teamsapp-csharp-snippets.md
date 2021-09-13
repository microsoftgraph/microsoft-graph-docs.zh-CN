---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f49da0d880b7e633c5eedec007592a2a8ce02d5066e83e97638321346ecefe25
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163738"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].Teamwork.InstalledApps["{userScopeTeamsAppInstallation-id}"]
    .Upgrade()
    .Request()
    .PostAsync();

```