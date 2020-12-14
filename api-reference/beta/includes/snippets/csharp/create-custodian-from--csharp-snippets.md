---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a8fb014eb22a5ccf4927cc9e17772147a2e6326
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659509"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var custodian = new Custodian
{
    Email = "AdeleV@contoso.com",
    ApplyHoldToSources = true
};

await graphClient.Compliance.Ediscovery.Cases["2192ca408ea2410eba3bec8ae873be6b"].Custodians
    .Request()
    .AddAsync(custodian);

```