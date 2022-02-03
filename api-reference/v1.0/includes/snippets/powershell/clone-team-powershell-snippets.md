---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d42372d82bef4b5f1645fd4961fa1c2376daa0a
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62342308"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    DisplayName = "Library Assist"
    Description = "Self help community for library"
    MailNickname = "libassist"
    PartsToClone = "apps,tabs,settings,channels,members"
    Visibility = "public"
}

Copy-MgTeam -TeamId $teamId -BodyParameter $params

```