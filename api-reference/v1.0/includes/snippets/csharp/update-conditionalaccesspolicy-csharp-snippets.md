---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db35041d457e4fadba34d7b8283e40ec92c6774f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781327"
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

await graphClient.Identity.ConditionalAccess.Policies["{conditionalAccessPolicy-id}"]
    .Request()
    .UpdateAsync(conditionalAccessPolicy);

```