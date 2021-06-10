---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd3d2bf6fc309b687e22b25f862d591bd5afd130
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869083"
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