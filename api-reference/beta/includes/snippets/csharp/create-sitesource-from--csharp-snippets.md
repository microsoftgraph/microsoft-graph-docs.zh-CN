---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbc5035978c76008a82ba35158c015cd2612c6a4
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659085"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var siteSource = new SiteSource
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"site@odata.bind", "https://graph.microsoft.com/v1.0/sites/{siteId}"}
    }
};

await graphClient.Compliance.Ediscovery.Cases["4c8f8f70-7785-4bd4-b296-c98376a2c5e1"].Custodians["2192ca408ea2410eba3bec8ae873be6b"].SiteSources
    .Request()
    .AddAsync(siteSource);

```