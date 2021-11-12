---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 40cf2499224734acfae2edbb34ee82ecdb6e1f19
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "60938783"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProviderBase = new AppleManagedIdentityProvider
{
    DisplayName = "Sign in with Apple",
    DeveloperId = "UBF8T346G9",
    ServiceId = "com.microsoft.rts.b2c.test.client",
    KeyId = "99P6D879C4",
    CertificateData = "******"
};

await graphClient.Identity.IdentityProviders
    .Request()
    .AddAsync(identityProviderBase);

```