---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7581eac32eb2ca9399e5b688d8b51420b2495cdb
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62134244"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    "@odata.type" = "#microsoft.graph.aadUserConversationMember"
    Roles = @(
        "owner"
    )
}

Update-MgTeamMember -TeamId $teamId -ConversationMemberId $conversationMemberId -BodyParameter $params

```