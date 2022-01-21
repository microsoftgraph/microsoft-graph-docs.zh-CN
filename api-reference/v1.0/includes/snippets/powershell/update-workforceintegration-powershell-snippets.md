---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a741983c4beae59c73916f5f502ec3e7ba75176
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62104127"
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
    SupportedEntities = "supportedEntities-value"
}

Update-MgTeamworkWorkforceIntegration -WorkforceIntegrationId $workforceIntegrationId -BodyParameter $params

```