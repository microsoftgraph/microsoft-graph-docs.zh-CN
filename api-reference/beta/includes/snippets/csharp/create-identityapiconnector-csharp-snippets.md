---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ea8c7c07eb364d4bb5f3104f1480468e43162ab
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51922583"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityApiConnector = new IdentityApiConnector
{
    DisplayName = "Test API",
    TargetUrl = "https://someotherapi.com/api",
    AuthenticationConfiguration = new Pkcs12Certificate
    {
        Pkcs12Value = "eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA",
        Password = "<password>"
    }
};

await graphClient.Identity.ApiConnectors
    .Request()
    .AddAsync(identityApiConnector);

```