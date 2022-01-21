---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9bde4c1c1ac8669f717821cfc11b2d02ac079c08
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62122268"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    "@odata.type" = "#microsoft.graph.countryNamedLocation"
    DisplayName = "Named location with unknown countries and regions"
    CountriesAndRegions = @(
        "US"
        "GB"
    )
    IncludeUnknownCountriesAndRegions = $true
}

New-MgIdentityConditionalAccessNamedLocation -BodyParameter $params

```