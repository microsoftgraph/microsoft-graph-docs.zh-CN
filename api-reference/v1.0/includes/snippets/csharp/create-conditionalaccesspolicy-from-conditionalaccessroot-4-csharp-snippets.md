---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6f9c31630605726c2297d49433fad71d6f8fde197e972d530e106be54331fed1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378787"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conditionalAccessPolicy = new ConditionalAccessPolicy
{
    DisplayName = "Require MFA to EXO from non-compliant devices.",
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