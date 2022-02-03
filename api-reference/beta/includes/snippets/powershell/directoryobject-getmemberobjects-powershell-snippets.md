---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93ae2d3028dc25ff980ff352c1bddc02e278fefb
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62346554"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    SecurityEnabledOnly = $true
}

# A UPN can also be used as -UserId.
Get-MgUserMemberObject -UserId $userId -BodyParameter $params

```