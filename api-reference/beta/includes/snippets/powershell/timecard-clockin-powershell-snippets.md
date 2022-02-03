---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd948ac268f650b3b17f3ee7d2082eb2044847df
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348207"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    AtAprovedLocation = $true
    Notes = @{
        ContentType = "text"
        Content = "clock in notes"
    }
}

Invoke-MgClockTeamScheduleTimeCardIn -TeamId $teamId -BodyParameter $params

```