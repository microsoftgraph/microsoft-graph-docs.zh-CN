---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ccdf1ad5cf96275b19df213cc14a09ecea7e183
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42593466"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var claimsMappingPolicy = await graphClient.Policies.ClaimsMappingPolicies["{id}"]
    .Request()
    .GetAsync();

```