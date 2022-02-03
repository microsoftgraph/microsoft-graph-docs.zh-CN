---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81007343d03856c735c9199756618f89e1991199
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62344074"
---
```powershell

Import-Module Microsoft.Graph.Compliance

$params = @{
    TagsToAdd = @(
        @{
            Id = "b4798d14-748d-468e-a1ec-96a2b1d49677"
        }
    )
}

Add-MgComplianceEdiscoveryCaseReviewSetQueryTag -CaseId $caseId -ReviewSetId $reviewSetId -ReviewSetQueryId $reviewSetQueryId -BodyParameter $params

```