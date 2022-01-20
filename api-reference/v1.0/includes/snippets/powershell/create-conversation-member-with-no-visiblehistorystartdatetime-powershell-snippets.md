---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e7ef7f07632fdc64007f6e681784d4442c6465c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62088792"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    "@odata.type" = "#microsoft.graph.aadUserConversationMember"
    "User@odata.bind" = "https://graph.microsoft.com/v1.0/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"
    Roles = @(
        "owner"
    )
}

New-MgChatMember -ChatId $chatId -BodyParameter $params

```