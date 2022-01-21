---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e7cc12707c9ead65ecf17d961e7ea3bcd317691a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62108068"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    DisplayName = "Finance"
    Members = @(
        @{
            UserId = "92f6952f-61ca-4a94-8910-508a240bc167"
        }
        @{
            UserId = "085d800c-b86b-4bfc-a857-9371ad1caf29"
        }
    )
}

New-MgTeamTag -TeamId $teamId -BodyParameter $params

```