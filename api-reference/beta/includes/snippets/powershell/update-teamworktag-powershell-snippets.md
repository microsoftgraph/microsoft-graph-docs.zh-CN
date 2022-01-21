---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e8b7cd68438b9f5d7d1e34e9333208310d83f67
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62122848"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    DisplayName = "Finance"
}

Update-MgTeamTag -TeamId $teamId -TeamworkTagId $teamworkTagId -BodyParameter $params

```