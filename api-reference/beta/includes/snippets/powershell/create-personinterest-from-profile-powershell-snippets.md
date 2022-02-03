---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94e1fecac48be599b2e12f3847f4d9116b1e7d4b
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350316"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Categories = @(
        "Sports"
    )
    Description = "World's greatest football club"
    DisplayName = "Chelsea FC"
    WebUrl = "https://www.chelseafc.com"
}

# A UPN can also be used as -UserId.
New-MgUserProfileInterest -UserId $userId -BodyParameter $params

```