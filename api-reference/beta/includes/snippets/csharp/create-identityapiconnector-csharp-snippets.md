---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d50fa5301a89b67d0c0b5e76caa0d6eed6ec45dde2bfc91b78064a3b53af845
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162488"
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