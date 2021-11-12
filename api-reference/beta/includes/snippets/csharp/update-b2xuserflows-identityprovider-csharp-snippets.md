---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d1b4ddbb49b67b252157a2b937b0c764671c4f3acc28e6d67a65fd3e8c9a51f1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162139"
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

await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"].IdentityProviders.References
    .Request()
    .AddAsync(identityProvider);

```