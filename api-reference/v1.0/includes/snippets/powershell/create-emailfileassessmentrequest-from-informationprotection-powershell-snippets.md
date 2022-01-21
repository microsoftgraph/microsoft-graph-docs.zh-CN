---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4980d781a403be37fb92a9ed8ed7a6c4b39b04fc
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62134696"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    "@odata.type" = "#microsoft.graph.emailFileAssessmentRequest"
    RecipientEmail = "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com"
    ExpectedAssessment = "block"
    Category = "malware"
    ContentData = "UmVjZWl2ZWQ6IGZyb20gTVcyUFIwME1CMDMxNC5uYW1wcmQwMC....."
}

New-MgInformationProtectionThreatAssessmentRequest -BodyParameter $params

```