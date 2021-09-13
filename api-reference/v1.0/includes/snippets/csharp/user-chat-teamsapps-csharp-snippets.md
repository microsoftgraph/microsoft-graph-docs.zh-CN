---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: babb1ef42c8c5c967c55cea4c3cb4e8c0bea448aa0336a301bc5052d101a111f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279300"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chat = await graphClient.Users["{user-id}"].Teamwork.InstalledApps["{userScopeTeamsAppInstallation-id}"].Chat
    .Request()
    .GetAsync();

```