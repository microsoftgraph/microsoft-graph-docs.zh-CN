---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97512313b268405f8f14e06188d62d58a5d7aa0c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62121434"
---
```powershell

Import-Module Microsoft.Graph.Security

$params = @{
    AssignedTo = "String"
    ClosedDateTime = [System.DateTime]::Parse("String (timestamp)")
    Comments = @(
        "String"
    )
    Feedback = "@odata.type: microsoft.graph.alertFeedback"
    Status = "@odata.type: microsoft.graph.alertStatus"
    Tags = @(
        "String"
    )
    VendorInformation = @{
        Provider = "String"
        Vendor = "String"
    }
}

Update-MgSecurityAlert -AlertId $alertId -BodyParameter $params

```