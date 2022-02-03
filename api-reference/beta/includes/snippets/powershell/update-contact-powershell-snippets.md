---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 450899f029b3acfcae5b85e337199ea83f18236c
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352101"
---
```powershell

Import-Module Microsoft.Graph.PersonalContacts

$params = @{
    EmailAddresses = @(
        @{
            Type = "personal"
            Name = "Pavel Bansky"
            Address = "pavelb@adatum.onmicrosoft.com"
        }
        @{
            Address = "pavelb@fabrikam.onmicrosoft.com"
            Name = "Pavel Bansky"
            Type = "other"
            OtherLabel = "Volunteer work"
        }
    )
}

# A UPN can also be used as -UserId.
Update-MgUserContact -UserId $userId -ContactId $contactId -BodyParameter $params

```