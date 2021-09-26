---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61ce29372e294257dc908975b1725466ea47b977
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59763800"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var claimsMappingPolicy = new ClaimsMappingPolicy
{
    DisplayName = "UpdateClaimsPolicy"
};

await graphClient.Policies.ClaimsMappingPolicies["{claimsMappingPolicy-id}"]
    .Request()
    .UpdateAsync(claimsMappingPolicy);

```