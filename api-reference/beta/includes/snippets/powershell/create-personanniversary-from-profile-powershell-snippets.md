---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 760ec6cc6b62545c67b833c19cd1873ceb8e2978
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349458"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Type = "birthday"
    Date = "1980-01-08"
}

# A UPN can also be used as -UserId.
New-MgUserProfileAnniversary -UserId $userId -BodyParameter $params

```