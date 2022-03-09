---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a368da76e712e1b08e4881130df64995b54acd1
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63394675"
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
                RestrictForAppsCreatedAfterDateTime = [System.DateTime]::Parse("2021-01-01T10:37:00Z")
            }
            @{
                RestrictionType = "passwordLifetime"
                MaxLifetime = "P4DT12H30M5S"
                RestrictForAppsCreatedAfterDateTime = [System.DateTime]::Parse("2017-01-01T10:37:00Z")
            }
            @{
                RestrictionType = "symmetricKeyAddition"
                MaxLifetime = $null
                RestrictForAppsCreatedAfterDateTime = [System.DateTime]::Parse("2021-01-01T10:37:00Z")
            }
            @{
                RestrictionType = "customPasswordAddition"
                MaxLifetime = $null
                RestrictForAppsCreatedAfterDateTime = [System.DateTime]::Parse("2015-01-01T10:37:00Z")
            }
            @{
                RestrictionType = "symmetricKeyLifetime"
                MaxLifetime = "P40D"
                RestrictForAppsCreatedAfterDateTime = [System.DateTime]::Parse("2015-01-01T10:37:00Z")
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