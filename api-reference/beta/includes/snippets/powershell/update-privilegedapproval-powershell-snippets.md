---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 347c8d549ff1637812ab35758409a46401793c3c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135398"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    ApprovalState = "approvalState-value"
    ApproverReason = "approverReason-value"
}

Update-MgPrivilegedApproval -PrivilegedApprovalId $privilegedApprovalId -BodyParameter $params

```