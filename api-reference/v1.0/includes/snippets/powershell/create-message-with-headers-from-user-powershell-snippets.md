---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 318b02f10490f3c8bb8a76c3a31261f27e1ede19
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351964"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    Subject = "9/8/2018: concert"
    Body = @{
        ContentType = "HTML"
        Content = "The group represents Washington."
    }
    ToRecipients = @(
        @{
            EmailAddress = @{
                Address = "AlexW@contoso.OnMicrosoft.com"
            }
        }
    )
    InternetMessageHeaders = @(
        @{
            Name = "x-custom-header-group-name"
            Value = "Washington"
        }
        @{
            Name = "x-custom-header-group-id"
            Value = "WA001"
        }
    )
}

# A UPN can also be used as -UserId.
New-MgUserMessage -UserId $userId -BodyParameter $params

```