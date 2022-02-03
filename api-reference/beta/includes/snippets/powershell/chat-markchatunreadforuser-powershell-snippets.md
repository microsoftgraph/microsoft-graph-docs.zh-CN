---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 01231f849a3d3789e22bda0881ccee95a99535d6
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348572"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    User = @{
        Id = "d864e79f-a516-4d0f-9fee-0eeb4d61fdc2"
    }
    TenantId = "2a690434-97d9-4eed-83a6-f5f13600199a"
    LastMessageReadDateTime = [System.DateTime]::Parse("2021-05-27T22:13:01.577Z")
}

Invoke-MgMarkChatUnread -ChatId $chatId -BodyParameter $params

```