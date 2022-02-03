---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4946d1a8c1084073426ea41f79a3c318a644430c
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352192"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Detail = @{
        ContentType = "text"
        Content = "I am originally from Australia, but grew up in Moscow, Russia."
    }
    DisplayName = "About Me"
}

# A UPN can also be used as -UserId.
New-MgUserProfileNote -UserId $userId -BodyParameter $params

```