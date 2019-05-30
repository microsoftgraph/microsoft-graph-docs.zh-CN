---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1f01754a701ba3ec1b5d390add319d8dcb093f5d
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34537091"
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
            DisabledPlans = new List<String>()
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