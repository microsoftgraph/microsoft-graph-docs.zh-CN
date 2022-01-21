---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 383c419bc9918b5b43be664ab807a13fa8fb838a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62122269"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    "@odata.type" = "#microsoft.graph.ipNamedLocation"
    DisplayName = "Untrusted IP named location"
    IsTrusted = $false
    IpRanges = @(
        @{
            "@odata.type" = "#microsoft.graph.iPv4CidrRange"
            CidrAddress = "12.34.221.11/22"
        }
        @{
            "@odata.type" = "#microsoft.graph.iPv6CidrRange"
            CidrAddress = "2001:0:9d38:90d6:0:0:0:0/63"
        }
    )
}

New-MgIdentityConditionalAccessNamedLocation -BodyParameter $params

```