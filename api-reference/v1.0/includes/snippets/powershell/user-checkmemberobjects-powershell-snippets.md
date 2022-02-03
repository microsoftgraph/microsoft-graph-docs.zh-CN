---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cec9b258b46021d052ccde9390516b6ab8479a09
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62346709"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    Ids = @(
        "80a963dd-84af-4eb8-b2a6-781e444d4fb0"
        "62e90394-69f5-4237-9190-012177145e10"
        "86a64f51-3a64-4cc6-a8c8-6b8f000c0f52"
        "ac38546e-ddf3-437a-ac5c-27a94cd7a0f1"
    )
}

# A UPN can also be used as -UserId.
Confirm-MgUserMemberObject -UserId $userId -BodyParameter $params

```