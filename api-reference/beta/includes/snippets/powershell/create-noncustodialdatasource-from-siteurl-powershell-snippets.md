---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8688261fc80ab053ef153f61e55999ba2d70b31c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100208"
---
```powershell

Import-Module Microsoft.Graph.Compliance

$params = @{
    ApplyHoldToSource = $false
    DataSource = @{
        "@odata.type" = "microsoft.graph.ediscovery.siteSource"
    }
}

New-MgComplianceEdiscoveryCaseNoncustodialDataSource -CaseId $caseId -BodyParameter $params

```