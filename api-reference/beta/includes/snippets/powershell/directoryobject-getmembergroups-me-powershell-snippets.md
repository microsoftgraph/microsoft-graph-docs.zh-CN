---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f2db61ecc992523431ca4ee7e22e03ecdd465d73
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62346933"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    SecurityEnabledOnly = $true
}

# A UPN can also be used as -UserId.
Get-MgUserMemberGroup -UserId $userId -BodyParameter $params

```