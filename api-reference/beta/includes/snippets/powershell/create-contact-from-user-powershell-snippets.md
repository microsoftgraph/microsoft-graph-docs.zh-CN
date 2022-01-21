---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 662612ca32374705cd6bb71ba67c3f62c0f0e51e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62119648"
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

New-MgUserContact -UserId $userId -BodyParameter $params

```