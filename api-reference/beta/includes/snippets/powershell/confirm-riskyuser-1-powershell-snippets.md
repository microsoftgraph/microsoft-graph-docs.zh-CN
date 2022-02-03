---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a06f302e2bb058362f4f451ea93a163a79262528
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340986"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    UserIds = @(
        "29f270bb-4d23-4f68-8a57-dc73dc0d4caf"
        "20f91ec9-d140-4d90-9cd9-f618587a1471"
    )
}

Confirm-MgRiskyUserCompromised -BodyParameter $params

```