---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ed0244d4f6021740676240711a03113d2db8ca04
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62134047"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    "@odata.type" = "#microsoft.graph.countryNamedLocation"
    DisplayName = "Updated named location without unknown countries and regions"
    CountriesAndRegions = @(
        "CA"
        "IN"
    )
    IncludeUnknownCountriesAndRegions = $false
}

Update-MgIdentityConditionalAccessNamedLocation -NamedLocationId $namedLocationId -BodyParameter $params

```