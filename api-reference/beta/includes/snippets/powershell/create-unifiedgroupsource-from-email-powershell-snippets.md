---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c8322f69033f5a49000a4921d40c78eb4361a16c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62103331"
---
```powershell

Import-Module Microsoft.Graph.Compliance

$params = @{
    Group = @{
        Mail = "SecretGroup@contoso.com"
    }
    IncludedSources = "mailbox, site"
}

New-MgComplianceEdiscoveryCaseCustodianUnifiedGroupSource -CaseId $caseId -CustodianId $custodianId -BodyParameter $params

```