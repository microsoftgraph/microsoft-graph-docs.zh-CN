---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fcff6f068f1b81ab66c4f8ac27e826a0bba8c0a8
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62087513"
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

New-MgUserContact -UserId $userId -BodyParameter $params

```