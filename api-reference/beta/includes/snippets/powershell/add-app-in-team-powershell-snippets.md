---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79890bbd89935e3f618ce7264d81f59c6ea9e058
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62108117"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    "TeamsApp@odata.bind" = "https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}

New-MgTeamInstalledApp -TeamId $teamId -BodyParameter $params

```