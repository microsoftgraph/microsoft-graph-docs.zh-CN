---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f6ee0ffb026bf3d0d649195ca7d1c7f587e6eee
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52081509"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProvider = new IdentityProvider
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/beta/identityProviders/{id}"}
    }
};

await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].IdentityProviders.References
    .Request()
    .AddAsync(identityProvider);

```