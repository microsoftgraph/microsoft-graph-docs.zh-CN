---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a06e6da5193d8f372da12c8d2d458d44e55a8198
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333445"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var servicePrincipal = new ServicePrincipal
{
    AppId = "65415bb1-9267-4313-bbf5-ae259732ee12"
};

await graphClient.Serviceprincipals
    .Request()
    .AddAsync(servicePrincipal);

```