---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e637778cae4ec3281a0acb8b5c75c957d7a737f8
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352634"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    AllowedAudiences = "contacts"
}

# A UPN can also be used as -UserId.
Update-MgUserProfileAnniversary -UserId $userId -PersonAnnualEventId $personAnnualEventId -BodyParameter $params

```