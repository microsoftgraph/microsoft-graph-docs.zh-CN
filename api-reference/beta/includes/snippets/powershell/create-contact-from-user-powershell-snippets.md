---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf10738565d5f80f7f3da39b40dfb0f8b3e5c8db
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351034"
---
```powershell

Import-Module Microsoft.Graph.PersonalContacts

$params = @{
    GivenName = "Pavel"
    Surname = "Bansky"
    EmailAddresses = @(
        @{
            Address = "pavelb@contoso.onmicrosoft.com"
            Name = "Pavel Bansky"
            Type = "personal"
        }
        @{
            Address = "pavelb@fabrikam.onmicrosoft.com"
            Name = "Pavel Bansky"
            Type = "other"
            OtherLabel = "Volunteer work"
        }
    )
    Phones = @(
        @{
            Number = "+1 732 555 0102"
            Type = "business"
        }
    )
}

# A UPN can also be used as -UserId.
New-MgUserContact -UserId $userId -BodyParameter $params

```