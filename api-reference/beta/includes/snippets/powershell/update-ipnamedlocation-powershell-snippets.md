---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 181a4460f4e20dce4bb0a035123ef7e70f6343c8
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62096391"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    "@odata.type" = "#microsoft.graph.ipNamedLocation"
    DisplayName = "Untrusted named location with only IPv4 address"
    IsTrusted = $false
    IpRanges = @(
        @{
            "@odata.type" = "#microsoft.graph.iPv4CidrRange"
            CidrAddress = "6.5.4.3/18"
        }
    )
}

Update-MgIdentityConditionalAccessNamedLocation -NamedLocationId $namedLocationId -BodyParameter $params

```