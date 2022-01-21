---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d4c7ee4b949d78e27bb890095f842c8704400790
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62093199"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    "@odata.id" = "https://graph.microsoft.com/beta/policies/claimsMappingPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}

New-MgServicePrincipalClaimMappingPolicyByRef -ServicePrincipalId $servicePrincipalId -BodyParameter $params

```