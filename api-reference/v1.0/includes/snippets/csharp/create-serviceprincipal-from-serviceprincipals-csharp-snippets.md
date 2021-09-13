---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e392fd55cda4f7b9b167042a824abe1249bf687322d2b6fac3574304a2199b13
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162332"
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