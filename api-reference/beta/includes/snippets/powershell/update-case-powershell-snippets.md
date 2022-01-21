---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3942beae760017a28c2399749f7272c31a728660
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62133866"
---
```powershell

Import-Module Microsoft.Graph.Compliance

$params = @{
    DisplayName = "My Case 1 - Renamed"
    Description = "Updated description"
    ExternalId = "Updated externalId"
}

Update-MgComplianceEdiscoveryCase -CaseId $caseId -BodyParameter $params

```