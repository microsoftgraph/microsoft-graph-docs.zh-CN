---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 119943db37e1d7c80d7a9c6d94ea8d3b5fa48eec
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62128959"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    Body = @{
        Content = "Hello world"
    }
}

New-MgChatMessage -ChatId $chatId -BodyParameter $params

```