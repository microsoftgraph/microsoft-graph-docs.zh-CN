---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1858f7a566d74941a96ec979deedf8b7b9479c57
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340074"
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
                    Address = "meganb@contoso.onmicrosoft.com"
                }
            }
        )
        Attachments = @(
            @{
                "@odata.type" = "#microsoft.graph.fileAttachment"
                Name = "attachment.txt"
                ContentType = "text/plain"
                ContentBytes = "SGVsbG8gV29ybGQh"
            }
        )
    }
}

# A UPN can also be used as -UserId.
Send-MgUserMail -UserId $userId -BodyParameter $params

```