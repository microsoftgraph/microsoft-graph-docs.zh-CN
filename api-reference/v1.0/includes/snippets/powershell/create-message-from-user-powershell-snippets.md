---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 573f49484e9cf67d11d163e0c0d01491c9c5ae4e
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351930"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    Subject = "Did you see last night's game?"
    Importance = "Low"
    Body = @{
        ContentType = "HTML"
        Content = "They were <b>awesome</b>!"
    }
    ToRecipients = @(
        @{
            EmailAddress = @{
                Address = "AdeleV@contoso.onmicrosoft.com"
            }
        }
    )
}

# A UPN can also be used as -UserId.
New-MgUserMessage -UserId $userId -BodyParameter $params

```