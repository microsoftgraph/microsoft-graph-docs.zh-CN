---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc0e79c5e5c501a3a8cf07779f7b631b54f112c85239d044647749fac0e023d6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105665"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authenticationMethodsPolicy = new AuthenticationMethodsPolicy
{
    RegistrationEnforcement = new RegistrationEnforcement
    {
        AuthenticationMethodsRegistrationCampaign = new AuthenticationMethodsRegistrationCampaign
        {
            SnoozeDurationInDays = 1,
            State = AdvancedConfigState.Enabled,
            ExcludeTargets = new List<ExcludeTarget>()
            {
            },
            IncludeTargets = new List<AuthenticationMethodsRegistrationCampaignIncludeTarget>()
            {
                new AuthenticationMethodsRegistrationCampaignIncludeTarget
                {
                    Id = "3ee3a9de-0a86-4e12-a287-9769accf1ba2",
                    TargetType = AuthenticationMethodTargetType.Group,
                    TargetedAuthenticationMethod = "microsoftAuthenticator"
                }
            }
        }
    }
};

await graphClient.Policies.AuthenticationMethodsPolicy
    .Request()
    .UpdateAsync(authenticationMethodsPolicy);

```