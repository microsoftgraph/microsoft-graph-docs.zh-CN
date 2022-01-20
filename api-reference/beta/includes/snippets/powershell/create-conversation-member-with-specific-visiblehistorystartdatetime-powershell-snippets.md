---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ff7848fc12f4d9f1038c287b67e273f540b1f28
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62121397"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    "@odata.type" = "#microsoft.graph.aadUserConversationMember"
    "User@odata.bind" = "https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"
    VisibleHistoryStartDateTime = [System.DateTime]::Parse("2019-04-18T23:51:43.255Z")
    Roles = @(
        "owner"
    )
}

New-MgChatMember -ChatId $chatId -BodyParameter $params

```