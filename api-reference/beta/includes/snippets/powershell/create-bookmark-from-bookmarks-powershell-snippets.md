---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0c3e9281d0ed2bbd12f32dfca36fc85a856cf5a
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338235"
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
            LanguageTag = "es-ES"
            DisplayName = "Sitio de instalación Contoso"
            Description = "Pruebe o compre Contoso hogar o negocios y vea la información del producto"
        }
    )
    GroupIds = @(
        "groupId"
    )
    PowerAppIds = @(
        "powerAppId"
    )
    State = "published"
}

New-MgSearchBookmark -BodyParameter $params

```