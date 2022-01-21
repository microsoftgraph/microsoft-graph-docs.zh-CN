---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f142846be7b5c7883d9c2666e19ee1b4e8687d97
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62090342"
---
```powershell

Import-Module Microsoft.Graph.Compliance

$params = @{
    DisplayName = "My Query 1 - Renamed"
}

Update-MgComplianceEdiscoveryCaseReviewSetQuery -CaseId $caseId -ReviewSetId $reviewSetId -ReviewSetQueryId $reviewSetQueryId -BodyParameter $params

```