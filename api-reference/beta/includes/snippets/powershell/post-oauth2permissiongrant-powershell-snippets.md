---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e69fc94d20f50f230f2fe4b1e47bf70db040de6
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758828"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    ClientId = "ef969797-201d-4f6b-960c-e9ed5f31dab5"
    ConsentType = "AllPrincipals"
    ResourceId = "943603e4-e787-4fe9-93d1-e30f749aae39"
    Scope = "DelegatedPermissionGrant.ReadWrite.All"
    StartTime = [System.DateTime]::Parse("2022-03-17T00:00:00Z")
    ExpiryTime = [System.DateTime]::Parse("2023-03-17T00:00:00Z")
}

New-MgOauth2PermissionGrant -BodyParameter $params

```