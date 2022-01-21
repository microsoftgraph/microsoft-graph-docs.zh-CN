---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f1e0f18d321e1df1b409a8f8c94ddb0824d1733
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62089012"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    DisplayName = "displayName-value"
    ApiVersion = 99
    Encryption = @{
        Protocol = "protocol-value"
        Secret = "secret-value"
    }
    IsActive = $true
    Url = "url-value"
    Supports = "supports-value"
}

New-MgTeamworkWorkforceIntegration -BodyParameter $params

```