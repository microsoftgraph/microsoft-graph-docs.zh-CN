---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 550a6ce0948638d939bff4b2aa8a014c4d4699d4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132438"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    Scope = "scope-value"
}

Update-MgOauth2PermissionGrant -OAuth2PermissionGrantId $oAuth2PermissionGrantId -BodyParameter $params

```