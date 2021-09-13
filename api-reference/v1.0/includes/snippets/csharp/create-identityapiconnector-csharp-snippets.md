---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 752501b88bf8a16764705b040e2b8322a44f9b3256cc79667a06cf15965d6e33
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219351"
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
        Password = "CertificatePassword"
    }
};

await graphClient.Identity.ApiConnectors
    .Request()
    .AddAsync(identityApiConnector);

```