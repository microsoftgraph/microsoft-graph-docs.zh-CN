---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0acd85ac5eba553beee7490a47618c2a388aee19
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340138"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    Reason = "reason-value"
    Duration = "duration-value"
    TicketNumber = "ticketNumber-value"
    TicketSystem = "ticketSystem-value"
}

Invoke-MgSelfPrivilegedRoleActivate -PrivilegedRoleId $privilegedRoleId -BodyParameter $params

```