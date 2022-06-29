---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c63fc61a5dc8bfa8a0dc668b8b8df3e7ec567e4
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447009"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    "@odata.type" = "#microsoft.graph.fido2AuthenticationMethodConfiguration"
    State = "enabled"
    IsAttestationEnforced = "true"
}

Update-MgPolicyAuthenticationMethodPolicyAuthenticationMethodConfiguration -AuthenticationMethodConfigurationId $authenticationMethodConfigurationId -BodyParameter $params

```