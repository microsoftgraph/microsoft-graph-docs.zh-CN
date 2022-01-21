---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c65caf370e158010a038695f4d382ea06a39eae8
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129659"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    ClientId = "clientId-value"
    ConsentType = "consentType-value"
    PrincipalId = "principalId-value"
    ResourceId = "resourceId-value"
    Scope = "scope-value"
    StartTime = [System.DateTime]::Parse("2016-10-19T10:37:00Z")
    ExpiryTime = [System.DateTime]::Parse("2016-10-19T10:37:00Z")
}

New-MgOauth2PermissionGrant -BodyParameter $params

```