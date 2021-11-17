---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4794305a9616c3279acdf434c1e415697a717259547f4daa11ba1de72d308c80
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164239"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userScopeTeamsAppInstallation = await graphClient.Users["{user-id}"].Teamwork.InstalledApps["{userScopeTeamsAppInstallation-id}"]
    .Request()
    .Expand("teamsAppDefinition")
    .GetAsync();

```