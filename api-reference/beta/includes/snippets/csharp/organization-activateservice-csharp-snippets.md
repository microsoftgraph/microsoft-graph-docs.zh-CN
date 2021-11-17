---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a651f5ef2cc752bff267083cefefe574fbd14af8226ce6e7bfbd6b93ae52828
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279133"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var skuId = Guid.Parse("6fd2c87f-b296-42f0-b197-1e91e994b900");

var servicePlanId = Guid.Parse("a23b959c-7ce8-4e57-9140-b90eb88a9e97");

await graphClient.Organization["{organization-id}"]
    .ActivateService(null,servicePlanId,skuId)
    .Request()
    .PostAsync();

```