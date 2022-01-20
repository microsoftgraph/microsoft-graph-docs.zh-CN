---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4fea646a890cbda13f48bd3b62c93441391c001
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62092604"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    "@odata.context" = "https://graph.microsoft.com/v1.0/$metadata#authenticationMethodsPolicy"
    RegistrationEnforcement = @{
        AuthenticationMethodsRegistrationCampaign = @{
            SnoozeDurationInDays = 1
            State = "enabled"
            ExcludeTargets = @(
            )
            IncludeTargets = @(
                @{
                    Id = "3ee3a9de-0a86-4e12-a287-9769accf1ba2"
                    TargetType = "group"
                    TargetedAuthenticationMethod = "microsoftAuthenticator"
                }
            )
        }
    }
    AuthenticationMethodConfigurations = @(
        @{
            "@odata.type" = "#microsoft.graph.fido2AuthenticationMethodConfiguration"
            Id = "Fido2"
            State = "disabled"
            IsSelfServiceRegistrationAllowed = $false
            IsAttestationEnforced = $false
        }
    )
}

Update-MgPolicyAuthenticationMethodPolicy -BodyParameter $params

```