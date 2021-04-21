---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a264ef5e3c61dec639f93e7b2fd01a8e66a78e8
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51922593"
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