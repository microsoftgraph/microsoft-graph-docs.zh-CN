---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 117d03d7c459b62644d7c04806c4d463aec1bc02
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62103330"
---
```powershell

Import-Module Microsoft.Graph.Compliance

$params = @{
    "Group@odata.bind" = "https://graph.microsoft.com/v1.0/groups/b96f95c5-b1b3-4142-b039-8ac79e7d2c84"
    IncludedSources = "mailbox, site"
}

New-MgComplianceEdiscoveryCaseCustodianUnifiedGroupSource -CaseId $caseId -CustodianId $custodianId -BodyParameter $params

```