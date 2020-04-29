---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 605f5d04908be7a0915be50dc3c11a6aee9b2b2e
ms.sourcegitcommit: 9b507499fb1ec61b4de47f36f915ae29c8594459
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2020
ms.locfileid: "43935222"
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
            IncludeDeviceStates = new List<String>()
            {
                "All"
            },
            ExcludeDeviceStates = new List<String>()
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