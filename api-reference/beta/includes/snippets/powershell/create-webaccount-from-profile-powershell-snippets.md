---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec0fa498e574ee933cd97f2fd5abf82f044b4de3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135189"
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

New-MgUserProfileWebAccount -UserId $userId -BodyParameter $params

```