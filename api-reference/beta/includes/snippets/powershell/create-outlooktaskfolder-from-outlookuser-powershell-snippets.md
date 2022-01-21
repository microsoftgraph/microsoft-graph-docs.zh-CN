---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f86041f128443430a34d7dae9a7bfa2600262322
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62123379"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    Name = "Volunteer"
}

New-MgUserOutlookTaskFolder -UserId $userId -BodyParameter $params

```