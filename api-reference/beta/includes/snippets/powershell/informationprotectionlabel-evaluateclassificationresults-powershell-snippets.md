---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 70511bf1cd05377f52b123666f2d9d8a800864ba
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62346869"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    ContentInfo = @{
        "@odata.type" = "#microsoft.graph.contentInfo"
        "Format@odata.type" = "#microsoft.graph.contentFormat"
        Format = "default"
        Identifier = $null
        "State@odata.type" = "#microsoft.graph.contentState"
        State = "rest"
    }
    ClassificationResults = @(
        @{
            SensitiveTypeId = "cb353f78-2b72-4c3c-8827-92ebe4f69fdf"
            Count = 4
            ConfidenceLevel = 75
        }
    )
}

Test-MgInformationProtectionPolicyLabelClassificationResult -BodyParameter $params

```