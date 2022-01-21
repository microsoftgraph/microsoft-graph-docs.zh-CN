---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a426f2257fee574bc6f7d9c320c22e9325bbf706
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62107368"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    Definition = @(
        "definition-value"
    )
    DisplayName = "displayName-value"
    IsOrganizationDefault = $true
}

New-MgPolicyTokenIssuancePolicy -BodyParameter $params

```