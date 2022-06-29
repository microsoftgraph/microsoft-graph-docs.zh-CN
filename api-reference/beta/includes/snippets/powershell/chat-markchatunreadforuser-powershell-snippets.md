---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 077bba72a906ff38a923d639c8c4629dccc2e05e
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66502419"
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

Invoke-MgMarkChatUnreadForUser -ChatId $chatId -BodyParameter $params

```