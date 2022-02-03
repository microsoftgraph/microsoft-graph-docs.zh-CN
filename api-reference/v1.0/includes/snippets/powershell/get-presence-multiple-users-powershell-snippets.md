---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbeb47132aeb8711050127039f8329de2a692e97
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347283"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    Ids = @(
        "fa8bf3dc-eca7-46b7-bad1-db199b62afc3"
        "66825e03-7ef5-42da-9069-724602c31f6b"
    )
}

Get-MgCommunicationPresence -BodyParameter $params

```