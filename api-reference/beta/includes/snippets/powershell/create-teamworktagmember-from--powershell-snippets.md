---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a904150d042b219fdba56123079afc4b9c582a2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118074"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    UserId = "97f62344-57dc-409c-88ad-c4af14158ff5"
}

New-MgTeamTagMember -TeamId $teamId -TeamworkTagId $teamworkTagId -BodyParameter $params

```