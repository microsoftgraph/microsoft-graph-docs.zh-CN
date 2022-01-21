---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd3dadbc4e0258371c4dfece5bcb2b36aba795bd
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62126208"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    ClientId = "clientId-value"
    ConsentType = "consentType-value"
    PrincipalId = "principalId-value"
    ResourceId = "resourceId-value"
    Scope = "scope-value"
}

New-MgOauth2PermissionGrant -BodyParameter $params

```