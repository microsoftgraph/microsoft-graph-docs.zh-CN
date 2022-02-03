---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c8dece9edc58395f7e821c6cbe7298bd04951e54
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62339721"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    Subject = "Annual review"
    Body = @{
        ContentType = "HTML"
        Content = "You should be proud!"
    }
    ToRecipients = @(
        @{
            EmailAddress = @{
                Address = "rufus@contoso.com"
            }
        }
    )
    Extensions = @(
        @{
            "@odata.type" = "microsoft.graph.openTypeExtension"
            ExtensionName = "Com.Contoso.Referral"
            CompanyName = "Wingtip Toys"
            ExpirationDate = "2015-12-30T11:00:00.000Z"
            DealValue = 
        }
    )
}

# A UPN can also be used as -UserId.
New-MgUserMessage -UserId $userId -BodyParameter $params

```