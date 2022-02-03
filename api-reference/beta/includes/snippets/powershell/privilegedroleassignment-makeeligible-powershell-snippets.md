---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc5b6a52050877984453a4ea9846a34c0eb12300
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62339690"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

New-MgPrivilegedRoleAssignmentEligible -PrivilegedRoleAssignmentId $privilegedRoleAssignmentId

```