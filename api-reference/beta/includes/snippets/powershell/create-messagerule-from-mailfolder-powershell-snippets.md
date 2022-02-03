---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e9f45a3c95d9d094f2a24d7c7d56257ccc38d77
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349586"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    DisplayName = "From partner"
    Sequence = 2
    IsEnabled = $true
    Conditions = @{
        SenderContains = @(
            "adele"
        )
    }
    Actions = @{
        ForwardTo = @(
            @{
                EmailAddress = @{
                    Name = "Alex Wilbur"
                    Address = "AlexW@contoso.onmicrosoft.com"
                }
            }
        )
        StopProcessingRules = $true
    }
}

# A UPN can also be used as -UserId.
New-MgUserMailFolderMessageRule -UserId $userId -MailFolderId $mailFolderId -BodyParameter $params

```