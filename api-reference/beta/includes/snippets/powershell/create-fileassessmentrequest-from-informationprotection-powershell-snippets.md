---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64ab6f0cff528dac027a4cbdf30c343200bee7c4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094048"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    "@odata.type" = "#microsoft.graph.fileAssessmentRequest"
    ExpectedAssessment = "block"
    Category = "malware"
    FileName = "test.txt"
    ContentData = "VGhpcyBpcyBhIHRlc3QgZmlsZQ=="
}

New-MgInformationProtectionThreatAssessmentRequest -BodyParameter $params

```