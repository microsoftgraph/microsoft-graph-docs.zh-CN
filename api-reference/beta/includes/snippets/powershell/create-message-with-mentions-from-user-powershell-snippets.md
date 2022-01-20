---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 466ca80f6a062d32465b2c659e8f4ae609c36a40
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62095720"
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

New-MgUserMessage -UserId $userId -BodyParameter $params

```