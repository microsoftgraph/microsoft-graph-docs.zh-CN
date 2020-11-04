---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be5f88ecdfdca069ce3f1a88ee43de429e95009e
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905509"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var servicePrincipals = await graphClient.ServicePrincipals
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Search("displayName:Team")
    .GetAsync();

```