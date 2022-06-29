---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b8e65bdf945dc136a7b87a4917e4254d14f3d53
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66502340"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    User = @{
        Id = "d864e79f-a516-4d0f-9fee-0eeb4d61fdc2"
    }
    TenantId = "2a690434-97d9-4eed-83a6-f5f13600199a"
}

Invoke-MgGraphChat -ChatId $chatId -BodyParameter $params

```