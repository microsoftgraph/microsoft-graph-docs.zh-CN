---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb5a91fcc91ace31c8cfbf1b159339eeb8dabdb7
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206876"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    "@odata.type" = "#microsoft.graph.aadUserConversationMember"
    Roles = @(
    )
    "User@odata.bind" = "https://graph.microsoft.com/beta/users/bc3598dd-cce4-4742-ae15-173429951408"
    TenantId = "a18103d1-a6ef-4f66-ac64-e4ef42ea8681"
}

New-MgTeamChannelMember -TeamId $teamId -ChannelId $channelId -BodyParameter $params

```