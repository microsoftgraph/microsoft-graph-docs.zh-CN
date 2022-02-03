---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f8a38bfef3b79a1003b90437f2e08541bd2422b
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349522"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    Subject = "Party planning"
    ToRecipients = @(
        @{
            EmailAddress = @{
                Name = "Samantha Booth"
                Address = "samanthab@contoso.onmicrosoft.com"
            }
        }
    )
    Mentions = @(
        @{
            Mentioned = @{
                Name = "Dana Swope"
                Address = "danas@contoso.onmicrosoft.com"
            }
        }
    )
}

# A UPN can also be used as -UserId.
New-MgUserMessage -UserId $userId -BodyParameter $params

```