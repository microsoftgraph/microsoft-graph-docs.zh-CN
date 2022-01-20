---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97273e66ce3dc0e561022014508afb1a60e2867a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130820"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    UserId = "userId-value"
    RoleId = "roleId-value"
}

New-MgPrivilegedRoleAssignment -BodyParameter $params

```