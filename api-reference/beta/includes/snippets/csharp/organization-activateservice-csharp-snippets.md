---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de7839b40250e87e47c2f354f1e839fd5ea985c1
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207664"
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