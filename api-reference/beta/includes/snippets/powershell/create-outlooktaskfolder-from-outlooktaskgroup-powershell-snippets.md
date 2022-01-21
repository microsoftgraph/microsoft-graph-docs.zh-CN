---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 45a00c5184cb9e032e01ac544eba8ac6bcd8e0c2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62108732"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    Name = "Cooking"
}

New-MgUserOutlookTaskGroupTaskFolder -UserId $userId -OutlookTaskGroupId $outlookTaskGroupId -BodyParameter $params

```