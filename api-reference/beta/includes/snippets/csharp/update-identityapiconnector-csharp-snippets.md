---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3892c6288caf0559d09192d3152ee6650181d8b4a193d400d54072ffe102fb8e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220672"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityApiConnector = new IdentityApiConnector
{
    AuthenticationConfiguration = new Pkcs12Certificate
    {
        Pkcs12Value = "eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA",
        Password = "secret"
    }
};

await graphClient.Identity.ApiConnectors["{identityApiConnector-id}"]
    .Request()
    .UpdateAsync(identityApiConnector);

```