---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce9643af7f90613eaf0241fdc133b72a8016ab2f
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350299"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    IsCurrent = $true
}

# A UPN can also be used as -UserId.
Update-MgUserProfilePosition -UserId $userId -WorkPositionId $workPositionId -BodyParameter $params

```