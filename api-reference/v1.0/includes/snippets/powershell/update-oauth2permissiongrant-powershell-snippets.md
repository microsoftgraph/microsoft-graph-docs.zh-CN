---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9bb94c5726897ed944a2cfbc4503ecc59986ce8f
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758829"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    Scope = "User.ReadBasic.All Group.ReadWrite.All"
}

Update-MgOauth2PermissionGrant -OAuth2PermissionGrantId $oAuth2PermissionGrantId -BodyParameter $params

```