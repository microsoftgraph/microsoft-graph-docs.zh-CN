---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85aa72b961f28d441e2859ee3440821eedd3dae7
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349461"
---
```powershell

Import-Module Microsoft.Graph.Notes

$params = @{
    DisplayName = "My Private notebook"
}

# A UPN can also be used as -UserId.
New-MgUserOnenoteNotebook -UserId $userId -BodyParameter $params

```