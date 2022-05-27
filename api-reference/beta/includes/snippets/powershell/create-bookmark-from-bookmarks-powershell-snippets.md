---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94bc4b321859421b91f1c974c7fb4db0e1509f0b
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65719296"
---
```powershell

Import-Module Microsoft.Graph.Search

$params = @{
    DisplayName = "Contoso Install Site"
    WebUrl = "http://www.contoso.com/"
    Description = "Try or buy Contoso for Home or Business and view product information"
    Keywords = @{
        Keywords = @(
            "Contoso"
            "install"
        )
        ReservedKeywords = @(
            "Contoso"
        )
        MatchSimilarKeywords = $true
    }
    AvailabilityStartDateTime = $null
    AvailabilityEndDateTime = $null
    Platforms = @(
        "windows"
    )
    TargetedVariations = @(
        @{
            LanguageTag = "es-es"
            DisplayName = "Sitio de instalación Contoso"
            Description = "Pruebe o compre Contoso hogar o negocios y vea la información del producto"
        }
    )
    State = "published"
}

New-MgSearchBookmark -BodyParameter $params

```