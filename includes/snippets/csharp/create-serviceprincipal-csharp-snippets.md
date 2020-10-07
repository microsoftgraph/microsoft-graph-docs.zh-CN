---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 28e48e4c9a019cc3e0d6fd79e3d013a037112ddb
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "48373296"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var servicePrincipal = new ServicePrincipal
{
    AppId = "d7fbfe28-c60e-46d2-8335-841923950d3b",
    Tags = new List<String>()
    {
        "WindowsAzureActiveDirectoryIntegratedApp",
        "WindowsAzureActiveDirectoryOnPremApp"
    }
};

await graphClient.Serviceprincipals
    .Request()
    .AddAsync(servicePrincipal);

```