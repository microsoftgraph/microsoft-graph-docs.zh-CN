---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d30f9d18a18b9065e108d2c0bbfb082c45ed6503
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844342"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityApiConnector = new IdentityApiConnector
{
    DisplayName = "New Test API",
    TargetUrl = "https://otherapi.com/api/endpoint",
    AuthenticationConfiguration = new BasicAuthentication
    {
        Username = "<NEW_USERNAME>",
        Password = "<NEW_PASSWORD>"
    }
};

await graphClient.Identity.ApiConnectors["{identityApiConnectorId}"]
    .Request()
    .UpdateAsync(identityApiConnector);

```