---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a10b3491d97e30c5f3f180e9fe4b3f8cefb0128a
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62345641"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    GroupIds = @(
        "fee2c45b-915a-4a64-b130-f4eb9e75525e"
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540"
    )
}

# A UPN can also be used as -UserId.
Confirm-MgUserMemberGroup -UserId $userId -BodyParameter $params

```