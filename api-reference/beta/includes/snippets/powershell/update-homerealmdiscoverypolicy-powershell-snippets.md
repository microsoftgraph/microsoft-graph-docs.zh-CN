---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9dc70ac8567901d4eee9a7c4adb6ff4dd8d66b5d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62127601"
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

Update-MgPolicyHomeRealmDiscoveryPolicy -HomeRealmDiscoveryPolicyId $homeRealmDiscoveryPolicyId -BodyParameter $params

```