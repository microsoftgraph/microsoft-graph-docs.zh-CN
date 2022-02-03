---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d103e9f8673a6e0839b6a7150432b0a5ddaa67d
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340072"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    Message = @{
        Subject = "Meet for lunch?"
        Body = @{
            ContentType = "Text"
            Content = "The new cafeteria is open."
        }
        ToRecipients = @(
            @{
                EmailAddress = @{
                    Address = "samanthab@contoso.onmicrosoft.com"
                }
            }
        )
        CcRecipients = @(
            @{
                EmailAddress = @{
                    Address = "danas@contoso.onmicrosoft.com"
                }
            }
        )
    }
    SaveToSentItems = "false"
}

# A UPN can also be used as -UserId.
Send-MgUserMail -UserId $userId -BodyParameter $params

```