---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a162d654c85cf586854d74d1e8a4343e802b834d
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340073"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    Message = @{
        Subject = "9/9/2018: concert"
        Body = @{
            ContentType = "HTML"
            Content = "The group represents Nevada."
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
                Value = "Nevada"
            }
            @{
                Name = "x-custom-header-group-id"
                Value = "NV001"
            }
        )
    }
}

# A UPN can also be used as -UserId.
Send-MgUserMail -UserId $userId -BodyParameter $params

```