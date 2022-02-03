---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8170cac007cf1763c90b0fd06c5f3701f565cb1e
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347558"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    Message = @{
        IsDeliveryReceiptRequested = $true
        ToRecipients = @(
            @{
                EmailAddress = @{
                    Address = "danas@contoso.onmicrosoft.com"
                    Name = "Dana Swope"
                }
            }
        )
    }
    Comment = "Dana, just want to make sure you get this."
}

# A UPN can also be used as -UserId.
Invoke-MgForwardUserMessage -UserId $userId -MessageId $messageId -BodyParameter $params

```