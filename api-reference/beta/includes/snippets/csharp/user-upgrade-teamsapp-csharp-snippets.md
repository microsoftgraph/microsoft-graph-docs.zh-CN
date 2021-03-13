---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 66bddabd5fb1c323c022b6975dc5e04bb57787f0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791710"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].Teamwork.InstalledApps["{userScopeTeamsAppInstallation-id}"]
    .Upgrade()
    .Request()
    .PostAsync();

```