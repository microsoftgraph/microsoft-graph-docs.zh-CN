---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a1165c85f7aaf5e7fea27ccd23041c1184447bf
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62110332"
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

New-MgUserMessage -UserId $userId -BodyParameter $params

```