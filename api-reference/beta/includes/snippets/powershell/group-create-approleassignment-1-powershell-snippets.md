---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d40f9ff93c65412bcf9c81bacf573c839e5cab1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62127691"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    PrincipalId = "7679d9a4-2323-44cd-b5c2-673ec88d8b12"
    ResourceId = "076e8b57-bac8-49d7-9396-e3449b685055"
    AppRoleId = "00000000-0000-0000-0000-000000000000"
}

New-MgGroupAppRoleAssignment -GroupId $groupId -BodyParameter $params

```