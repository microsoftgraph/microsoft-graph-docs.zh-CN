---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81fb0a11ea393cf2591752ee265c174b7f589da6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62126340"
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

New-MgUserMailFolderMessageRule -UserId $userId -MailFolderId $mailFolderId -BodyParameter $params

```