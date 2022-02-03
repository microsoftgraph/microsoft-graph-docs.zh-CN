---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 299d896abf1e29a3fc4b3e8bf31361f6b4fb1de4
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351334"
---
```powershell

Import-Module Microsoft.Graph.PersonalContacts

$params = @{
    GivenName = "Pavel"
    Surname = "Bansky"
    EmailAddresses = @(
        @{
            Address = "pavelb@fabrikam.onmicrosoft.com"
            Name = "Pavel Bansky"
        }
    )
    BusinessPhones = @(
        "+1 732 555 0102"
    )
}

# A UPN can also be used as -UserId.
New-MgUserContact -UserId $userId -BodyParameter $params

```