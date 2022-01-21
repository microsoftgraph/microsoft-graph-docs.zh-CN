---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4cad079d7b1e364df6a31e1a6c23303af011c1e5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62128888"
---
```powershell

Import-Module Microsoft.Graph.PersonalContacts

$params = @{
    HomeAddress = @{
        Street = "123 Some street"
        City = "Seattle"
        State = "WA"
        PostalCode = "98121"
    }
    Birthday = [System.DateTime]::Parse("1974-07-22")
}

Update-MgUserContact -UserId $userId -ContactId $contactId -BodyParameter $params

```