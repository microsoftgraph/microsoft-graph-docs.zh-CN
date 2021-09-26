---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 59466a86b407212d604c585f415a796352ff799e
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59763898"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalDomainName = new ExternalDomainName
{
    Id = "contososuites.com"
};

await graphClient.Directory.FederationConfigurations["{identityProviderBase-id}"].Domains
    .Request()
    .AddAsync(externalDomainName);

```