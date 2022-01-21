---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0049b49b419e1bfbed8f178e92003bac8b9bb957
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62091519"
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

Update-MgPolicyTokenIssuancePolicy -TokenIssuancePolicyId $tokenIssuancePolicyId -BodyParameter $params

```