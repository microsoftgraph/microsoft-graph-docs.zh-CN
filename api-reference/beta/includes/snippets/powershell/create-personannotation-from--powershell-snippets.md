---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c00f176b97e609236e26cdd5c005a23101c1f92
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132816"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Detail = @{
        ContentType = "text"
        Content = "I am originally from Australia, but grew up in Moscow, Russia."
    }
    DisplayName = "About Me"
}

New-MgUserProfileNote -UserId $userId -BodyParameter $params

```