---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a2bfdf2d3449aa987907bf5df2464ee80897dfaa
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341652"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    Message = @{
        ToRecipients = @(
            @{
                EmailAddress = @{
                    Address = "samanthab@contoso.onmicrosoft.com"
                    Name = "Samantha Booth"
                }
            }
            @{
                EmailAddress = @{
                    Address = "randiw@contoso.onmicrosoft.com"
                    Name = "Randi Welch"
                }
            }
        )
    }
    Comment = "Samantha, Randi, would you name the group if the project is approved, please?"
}

# A UPN can also be used as -UserId.
New-MgUserMessageReply -UserId $userId -MessageId $messageId -BodyParameter $params

```