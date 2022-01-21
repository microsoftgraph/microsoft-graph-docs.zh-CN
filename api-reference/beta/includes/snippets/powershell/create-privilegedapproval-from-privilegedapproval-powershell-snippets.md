---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 015742c36023f57a92074c974d35f96d41812b88
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62112234"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    UserId = "userId-value"
    RoleId = "roleId-value"
    ApprovalType = "approvalType-value"
    ApprovalState = "approvalState-value"
    ApprovalDuration = "datetime-value"
}

New-MgPrivilegedApproval -BodyParameter $params

```