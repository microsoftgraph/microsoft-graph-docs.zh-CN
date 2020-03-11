---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 350ab9de9199754daf974cdf5bf7ea096ff27c1e
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42593529"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var claimsMappingPolicies = await graphClient.Policies.ClaimsMappingPolicies
    .Request()
    .GetAsync();

```