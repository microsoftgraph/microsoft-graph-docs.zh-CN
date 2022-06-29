---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88776ad77aa26ab06ee1b98d0618494e03f01f75
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437229"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    "@odata.type" = "#microsoft.graph.x509CertificateAuthenticationMethodConfiguration"
    Id = "X509Certificate"
    State = "enabled"
    CertificateUserBindings = @(
    )
    IncludeTargets = @(
    )
}

Update-MgPolicyAuthenticationMethodPolicyAuthenticationMethodConfiguration -AuthenticationMethodConfigurationId $authenticationMethodConfigurationId -BodyParameter $params

```