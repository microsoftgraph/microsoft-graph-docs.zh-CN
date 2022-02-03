---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8a623613518859e2a8d662328fafa79de54875a
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341601"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    Id = "id-value"
    GroupId = "groupId-value"
}

# A UPN can also be used as -UserId.
Copy-MgUserOnenotePageToSection -UserId $userId -OnenotePageId $onenotePageId -BodyParameter $params

```