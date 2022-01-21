---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0eafcb1133ed478b301f0f14ce1109b0018b52dc
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135259"
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

New-MgUserProfileInterest -UserId $userId -BodyParameter $params

```