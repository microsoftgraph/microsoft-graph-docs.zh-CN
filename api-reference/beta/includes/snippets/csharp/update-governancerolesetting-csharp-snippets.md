---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 860575e195be682d3d8298895b6874eaff38117e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797352"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var governanceRoleSetting = new GovernanceRoleSetting
{
    AdminEligibleSettings = new List<GovernanceRuleSetting>()
    {
        new GovernanceRuleSetting
        {
            RuleIdentifier = "ExpirationRule",
            Setting = "{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}"
        }
    }
};

await graphClient.PrivilegedAccess["{privilegedAccess-id}"].RoleSettings["{governanceRoleSetting-id}"]
    .Request()
    .UpdateAsync(governanceRoleSetting);

```