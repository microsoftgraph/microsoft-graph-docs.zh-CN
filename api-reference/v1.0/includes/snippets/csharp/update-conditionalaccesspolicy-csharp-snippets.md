---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eaae0779b18198d0a0476f3dd459ddb0f0237760
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566058"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conditionalAccessPolicy = new ConditionalAccessPolicy
{
    Conditions = new ConditionalAccessConditionSet
    {
        SignInRiskLevels = new List<RiskLevel>()
        {
            RiskLevel.High,
            RiskLevel.Medium,
            RiskLevel.Low
        }
    }
};

await graphClient.Identity.ConditionalAccess.Policies["{id}"]
    .Request()
    .UpdateAsync(conditionalAccessPolicy);

```