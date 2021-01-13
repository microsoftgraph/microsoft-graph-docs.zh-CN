---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e33266ec3e21a424c7322d923c85d6548f2f3613
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844546"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityApiConnector = new IdentityApiConnector
{
    DisplayName = "Test API",
    TargetUrl = "https://someapi.com/api",
    AuthenticationConfiguration = new BasicAuthentication
    {
        Username = "<USERNAME>",
        Password = "<PASSWORD>"
    }
};

await graphClient.Identity.ApiConnectors
    .Request()
    .AddAsync(identityApiConnector);

```