---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bed666f51f8579697a78e811c3d0d365583925e7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792594"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conditionalAccessPolicy = new ConditionalAccessPolicy
{
    DisplayName = "Require MFA to EXO from non-complaint devices.",
    State = ConditionalAccessPolicyState.Enabled,
    Conditions = new ConditionalAccessConditionSet
    {
        Applications = new ConditionalAccessApplications
        {
            IncludeApplications = new List<String>()
            {
                "00000002-0000-0ff1-ce00-000000000000"
            }
        },
        Users = new ConditionalAccessUsers
        {
            IncludeGroups = new List<String>()
            {
                "ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba"
            }
        },
        Devices = new ConditionalAccessDevices
        {
            IncludeDevices = new List<String>()
            {
                "All"
            },
            ExcludeDevices = new List<String>()
            {
                "Compliant"
            }
        }
    },
    GrantControls = new ConditionalAccessGrantControls
    {
        Operator = "OR",
        BuiltInControls = new List<ConditionalAccessGrantControl>()
        {
            ConditionalAccessGrantControl.Mfa
        }
    }
};

await graphClient.Identity.ConditionalAccess.Policies
    .Request()
    .AddAsync(conditionalAccessPolicy);

```