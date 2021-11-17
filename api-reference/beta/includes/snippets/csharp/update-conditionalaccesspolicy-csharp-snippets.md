---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c1fe0f6111ea0b63155bbf14fc89cd2cf36af62223780c6036606a5c31c0ee60
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105233"
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