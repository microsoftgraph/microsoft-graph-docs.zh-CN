---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f13e7ac4a763380d1c4458664ae8d5427de34dcf
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63759021"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    ClientId = "ef969797-201d-4f6b-960c-e9ed5f31dab5"
    ConsentType = "AllPrincipals"
    ResourceId = "943603e4-e787-4fe9-93d1-e30f749aae39"
    Scope = "DelegatedPermissionGrant.ReadWrite.All"
}

New-MgOauth2PermissionGrant -BodyParameter $params

```