---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 857eb42a7b87dd58064c16ad3178b32c95232c9b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62127979"
---
```powershell

Import-Module Microsoft.Graph.Compliance

$params = @{
    DisplayName = "Privileged"
    Description = "The document is privileged"
    "Parent@odata.bind" = "https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/98fdad78bbce4519b75474bc150575c3"
}

New-MgComplianceEdiscoveryCaseTag -CaseId $caseId -BodyParameter $params

```