---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0bf13eb44ee65d22bdd33c1ca308e11faa21df34
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447268"
---
```powershell

Import-Module Microsoft.Graph.Security

$params = @{
    "@odata.type" = "#microsoft.graph.security.ediscoveryCaseSettings"
    RedundancyDetection = @{
        "@odata.type" = "microsoft.graph.security.redundancyDetectionSettings"
    }
    TopicModeling = @{
        "@odata.type" = "microsoft.graph.security.topicModelingSettings"
    }
    Ocr = @{
        "@odata.type" = "microsoft.graph.security.ocrSettings"
    }
}

Update-MgSecurityCaseEdiscoveryCaseSetting -EdiscoveryCaseId $ediscoveryCaseId -BodyParameter $params

```