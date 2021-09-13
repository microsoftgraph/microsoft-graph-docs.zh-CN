---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44c04caa9f57e10c0163275414db9fb55dcfdb003290cb6e55700171f6fb0134
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378789"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conditionalAccessPolicy = new ConditionalAccessPolicy
{
    DisplayName = "Access to EXO requires MFA",
    State = ConditionalAccessPolicyState.Enabled,
    Conditions = new ConditionalAccessConditionSet
    {
        ClientAppTypes = new List<ConditionalAccessClientApp>()
        {
            ConditionalAccessClientApp.MobileAppsAndDesktopClients,
            ConditionalAccessClientApp.Browser
        },
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
        Locations = new ConditionalAccessLocations
        {
            IncludeLocations = new List<String>()
            {
                "All"
            },
            ExcludeLocations = new List<String>()
            {
                "AllTrusted"
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