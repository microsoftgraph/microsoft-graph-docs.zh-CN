---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31484a7281bdde47f3cdb6e873e20ec06bba947e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100207"
---
```powershell

Import-Module Microsoft.Graph.Compliance

$params = @{
    ApplyHoldToSource = $true
    DataSource = @{
        "@odata.type" = "microsoft.graph.ediscovery.userSource"
        Email = "adelev@contoso.com"
    }
}

New-MgComplianceEdiscoveryCaseNoncustodialDataSource -CaseId $caseId -BodyParameter $params

```