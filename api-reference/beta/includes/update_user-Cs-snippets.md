---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fc539e70c96eb46451a17bd1bd9df1b863edb11e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34475834"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = new User
{
    AccountEnabled = true,
    AssignedLicenses = new List<AssignedLicense>()
    {
        new AssignedLicense
        {
            DisabledPlans = new List<Guid>()
            {
                "bea13e0c-3828-4daa-a392-28af7ff61a0f"
            },
            SkuId = "skuId-value"
        }
    },
    AssignedPlans = new List<AssignedPlan>()
    {
        new AssignedPlan
        {
            AssignedDateTime = "2016-10-19T10:37:00Z",
            CapabilityStatus = "capabilityStatus-value",
            Service = "service-value",
            ServicePlanId = "bea13e0c-3828-4daa-a392-28af7ff61a0f"
        }
    },
    BusinessPhones = new List<String>()
    {
        "businessPhones-value"
    },
    City = "city-value"
};

await graphClient.Me
    .Request()
    .UpdateAsync(user);

```