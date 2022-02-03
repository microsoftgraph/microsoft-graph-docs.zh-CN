---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ee8dce5f06527170c502d7702890cf16c1abb467
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351155"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Description = "My Github contributions!"
    UserId = "innocenty.popov"
    Service = @{
        Name = "GitHub"
        WebUrl = "https://github.com"
    }
}

# A UPN can also be used as -UserId.
New-MgUserProfileWebAccount -UserId $userId -BodyParameter $params

```