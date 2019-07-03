---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d6d45ece72e7986c2759d68b5c171c14a8ee2b95
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520592"
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

await graphClient.PrivilegedAccess["pimforazurerbac"].RoleSettings["5fb5aef8-1081-4b8e-bb16-9d5d0385bab5"]
    .Request()
    .UpdateAsync(governanceRoleSetting);

```