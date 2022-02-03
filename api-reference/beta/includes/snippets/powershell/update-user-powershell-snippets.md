---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eca9fd741c64cece3e64458a8195800e551df320
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62342532"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    BusinessPhones = @(
        "+1 425 555 0109"
    )
    OfficeLocation = "18/2111"
}

# A UPN can also be used as -UserId.
Update-MgUser -UserId $userId -BodyParameter $params

```