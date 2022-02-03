---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90094d5f7e4080fda2f35a0c72f0046eff66cc9a
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349904"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    Name = "Cooking"
}

# A UPN can also be used as -UserId.
New-MgUserOutlookTaskGroupTaskFolder -UserId $userId -OutlookTaskGroupId $outlookTaskGroupId -BodyParameter $params

```