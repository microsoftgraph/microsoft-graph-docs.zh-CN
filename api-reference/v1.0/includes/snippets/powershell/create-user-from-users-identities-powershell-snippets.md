---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62de43ae764f1dff798b5a46e9612a1a6c4543c1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114651"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    DisplayName = "John Smith"
    Identities = @(
        @{
            SignInType = "userName"
            Issuer = "contoso.onmicrosoft.com"
            IssuerAssignedId = "johnsmith"
        }
        @{
            SignInType = "emailAddress"
            Issuer = "contoso.onmicrosoft.com"
            IssuerAssignedId = "jsmith@yahoo.com"
        }
        @{
            SignInType = "federated"
            Issuer = "facebook.com"
            IssuerAssignedId = "5eecb0cd"
        }
    )
    PasswordProfile = @{
        Password = "password-value"
        ForceChangePasswordNextSignIn = $false
    }
    PasswordPolicies = "DisablePasswordExpiration"
}

New-MgUser -BodyParameter $params

```