---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5de3137024699fe62330bf02bfa28d5379b4db51
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349906"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    DisplayName = "Clutter"
    IsHidden = $true
}

# A UPN can also be used as -UserId.
New-MgUserMailFolder -UserId $userId -BodyParameter $params

```