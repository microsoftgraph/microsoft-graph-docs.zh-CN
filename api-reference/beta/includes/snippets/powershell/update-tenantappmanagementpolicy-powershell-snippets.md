---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c9d6f215a1a93705cb1ca553fcb0cd752fea5bf0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62098493"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    IsEnabled = $true
    ApplicationRestrictions = @{
        PasswordCredentials = @(
            @{
                RestrictionType = "passwordAddition"
                MaxLifetime = $null
                RestrictForAppsCreatedAfterDateTime = [System.DateTime]::Parse("2021-04-01T10:37:00Z")
            }
            @{
                RestrictionType = "passwordLifetime"
                MaxLifetime = "P4DT12H30M5S"
                RestrictForAppsCreatedAfterDateTime = [System.DateTime]::Parse("2019-01-01T10:37:00Z")
            }
            @{
                RestrictionType = "symmetricKeyAddition"
                MaxLifetime = $null
                RestrictForAppsCreatedAfterDateTime = [System.DateTime]::Parse("2021-04-01T10:37:00Z")
            }
            @{
                RestrictionType = "symmetricKeyLifetime"
                MaxLifetime = "P40D"
                RestrictForAppsCreatedAfterDateTime = [System.DateTime]::Parse("2015-04-01T10:37:00Z")
            }
        )
        KeyCredentials = @(
            @{
                RestrictionType = "asymmetricKeyLifetime"
                MaxLifetime = "P30D"
                RestrictForAppsCreatedAfterDateTime = [System.DateTime]::Parse("2015-01-01T10:37:00Z")
            }
        )
    }
}

Update-MgPolicyDefaultAppManagementPolicy -BodyParameter $params

```