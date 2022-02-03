---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29e9266d0e686c955023b0c27cf419ec822769fc
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340124"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    Reason = "reason-value"
    TicketNumber = "ticketNumber-value"
    TicketSystem = "ticketSystem-value"
}

New-MgPrivilegedRoleAssignmentPermanent -PrivilegedRoleAssignmentId $privilegedRoleAssignmentId -BodyParameter $params

```