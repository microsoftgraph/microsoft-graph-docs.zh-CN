---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c060628e94f6501d2543e1eaf8517a385626b61c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094222"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    "@odata.id" = "https://graph.microsoft.com/beta/users/0f933635-5b77-4cf4-a577-f78a5eb090a2"
}

New-MgDirectoryRoleMemberByRef -DirectoryRoleId $directoryRoleId -BodyParameter $params

```