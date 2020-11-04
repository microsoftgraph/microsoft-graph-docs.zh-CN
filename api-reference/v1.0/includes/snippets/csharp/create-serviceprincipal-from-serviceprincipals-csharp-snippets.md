---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06faa69f714caa04de4eed3e4111ea2339f76381
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905378"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var servicePrincipal = new ServicePrincipal
{
    AppId = "65415bb1-9267-4313-bbf5-ae259732ee12"
};

await graphClient.ServicePrincipals
    .Request()
    .AddAsync(servicePrincipal);

```