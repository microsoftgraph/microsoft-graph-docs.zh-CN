---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ea122d6b211703df2ea40ce5fde5ba4a768b99c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62128139"
---
```powershell

Import-Module Microsoft.Graph.Calendar

$params = @{
    Name = "Volunteer"
}

New-MgUserCalendar -UserId $userId -BodyParameter $params

```