---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4bd015bcaeba04c5000688819124926225917daf
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116758"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
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
}

Update-MgPolicyAuthenticationMethodPolicy -BodyParameter $params

```