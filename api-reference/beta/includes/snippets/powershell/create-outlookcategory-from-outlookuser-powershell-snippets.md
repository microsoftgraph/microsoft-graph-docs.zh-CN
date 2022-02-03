---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06352c0bfa72e65e8ed0bdd46ae7d3d44eb1f537
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352320"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    DisplayName = "Project expenses"
    Color = "preset9"
}

# A UPN can also be used as -UserId.
New-MgUserOutlookMasterCategory -UserId $userId -BodyParameter $params

```