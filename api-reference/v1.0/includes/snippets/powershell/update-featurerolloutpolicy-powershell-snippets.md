---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26163bbc6a415e28c102a61307b84fcd6f396f44
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100871"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    DisplayName = "PasswordHashSync Rollout Policy"
    Description = "PasswordHashSync Rollout Policy"
    IsEnabled = $true
    IsAppliedToOrganization = $false
}

Update-MgPolicyFeatureRolloutPolicy -FeatureRolloutPolicyId $featureRolloutPolicyId -BodyParameter $params

```