---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: daaa002715a3118fa102214856e82e5cf6755196
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62339088"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    StorageLocation = "storageLocation-value"
}

Export-MgUserPersonalData -UserId $userId -BodyParameter $params

```