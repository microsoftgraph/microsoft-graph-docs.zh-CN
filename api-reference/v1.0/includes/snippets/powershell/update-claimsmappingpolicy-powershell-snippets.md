---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bfcb7afd90a26c1b0704a8015d51515a431ff890
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62117920"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    DisplayName = "UpdateClaimsPolicy"
}

Update-MgPolicyClaimMappingPolicy -ClaimsMappingPolicyId $claimsMappingPolicyId -BodyParameter $params

```